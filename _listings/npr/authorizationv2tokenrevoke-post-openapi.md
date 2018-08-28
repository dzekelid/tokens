---
swagger: "2.0"
x-collection-name: NPR
x-complete: 0
info:
  title: NPR Revoke an existing OAuth2 access token
  description: |-
    Our implementation follows the proposed IETF specification [RFC-7009](https://tools.ietf.org/html/rfc7009).

    If your client application offers the ability to for a logged-in user to log out, and you have access to a long-lived
    `client_credentials` token (i.e. you have generated one that you are storing securely for the lifetime of the entire app
    install), we suggest (but do not require) that you call this endpoint and revoke the access token belonging to the
    logged-in user as part of your logout process. If you do not already have a long-lived `client_credentials` token,
    please don't generate one just for the purposes of calling this endpoint.

    If you are building a prototype application, we also recommend that you use this endpoint to clean up access tokens
    that you generate during the testing of your app and do not intend to reuse.

    Note that revoking an access token will automatically revoke any refresh tokens associated with it, and vice-versa.
  termsOfService: http://dev.npr.org/develop/terms-of-use
  contact:
    name: NPR One Enterprise Team
    url: http://dev.npr.org
    email: NPROneEnterprise@npr.org
  version: 1.0.0
host: api.npr.org
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /authorization/v2/token:
    post:
      summary: Create a new OAuth2 access token
      description: |-
        Please be aware that the required parameters are contingent on the `grant_type` that you select.

        For the `authorization_code` grant type, you are **required** to pass in the `code` and `redirect_uri` parameters. `service`, `username` and `password` parameters will be ignored.

        For the `client_credentials` grant type, you do not need to pass in any additional parameters beyond the basic requirements. `code`, `redirect_uri`, `service`, `username` and `password` parameters will be ignored.

        For the `device_code` grant type, you are **required** to pass in the `code` parameter. `redirect_uri`, `service`, `username` and `password` parameters will be ignored.

        For the `password` grant type, you are **required** to pass in the `username` and `password` parameters. If you are logging in via a social service, you should also pass in the `service` parameter. (In this case, the access token you receive from the social service will serve as both your username and password.) The `code` and `redirect_uri` parameters are ignored.
        Third-party developers do not have access to this grant type.

        For the `refresh_token` grant type, you are **required** to pass in the `refresh_token` parameter. The `scope` parameter can optionally be used to request a different set of scopes than were used in the original request, but it **cannot** contain any scopes that were not previously requested. If not specified, then `scope` will be set to whichever scopes were used for the original access token request. If trading in an old non-expiring access token for a refresh-enabled token, set the value of `refresh_token` to the access token value and `token_type_hint` must be set to `access_token`. `code`, `redirect_uri`, `service`, `username` and `password` parameters will be ignored.

        The `temporary_user` and `anonymous_user` grant types are custom grant types created by NPR to suit our needs for functionality such as our &quot;try-before-you-buy&quot; experience. If you are a third-party developer, you will not have access to these grant types unless we have explicitly given you permission within our system.
        For these grant types, you do not need to pass in any additional parameters beyond the basic requirements. `code`, `redirect_uri`, `service`, `username` and `password` parameters will be ignored.

        If you are unsure of which grant type to select, assume that `authorization_code` is the one you want.

        Note that at this time, refresh tokens are an opt-in feature; however, in the future, they will gradually transition to being opt-out, and ultimately required for all clients. Our general guidance at this time is that if this endpoint starts returning refresh tokens for you, you are responsible for implementing the code to handle them appropriately in accordance with the OAuth 2.0 spec. For more information about our gradual rollout of this feature, please contact the NPR One API team.
      operationId: createToken
      x-api-path-slug: authorizationv2token-post
      parameters:
      - in: formData
        name: client_id
        description: The clients ID, required for all grant types
      - in: formData
        name: client_secret
        description: The clients secret, required for all grant types
      - in: formData
        name: code
        description: Required for `authorization_code` and `device_code` grant types
      - in: formData
        name: grant_type
        description: The type of grant the client is requesting
      - in: formData
        name: password
        description: Required for `password` grant type
      - in: formData
        name: redirect_uri
        description: Required for `authorization_code` grant type
      - in: formData
        name: refresh_token
        description: Required for `refresh_token` grant type
      - in: formData
        name: scope
        description: Optionally used by the `refresh_token` grant type only
      - in: formData
        name: service
        description: If logging in via a social service, this parameter should be
          set
      - in: formData
        name: token_type_hint
        description: A hint about the type of the token submitted for a new access
          and refresh token
      - in: formData
        name: username
        description: Required for `password` grant type
      responses:
        200:
          description: OK
      tags:
      - News
      - Authorization
      - Token
  /authorization/v2/token/revoke:
    post:
      summary: Revoke an existing OAuth2 access token
      description: |-
        Our implementation follows the proposed IETF specification [RFC-7009](https://tools.ietf.org/html/rfc7009).

        If your client application offers the ability to for a logged-in user to log out, and you have access to a long-lived
        `client_credentials` token (i.e. you have generated one that you are storing securely for the lifetime of the entire app
        install), we suggest (but do not require) that you call this endpoint and revoke the access token belonging to the
        logged-in user as part of your logout process. If you do not already have a long-lived `client_credentials` token,
        please don't generate one just for the purposes of calling this endpoint.

        If you are building a prototype application, we also recommend that you use this endpoint to clean up access tokens
        that you generate during the testing of your app and do not intend to reuse.

        Note that revoking an access token will automatically revoke any refresh tokens associated with it, and vice-versa.
      operationId: revokeToken
      x-api-path-slug: authorizationv2tokenrevoke-post
      parameters:
      - in: header
        name: Authorization
        description: A `client_credentials` access token from the same client application
          as the token being revoked
      - in: formData
        name: token
        description: The access token or refresh token that the client wants to have
          revoked
      - in: formData
        name: token_type_hint
        description: A hint about the type of the token submitted for revocation
      responses:
        200:
          description: OK
      tags:
      - News
      - Authorization
      - Token
      - Revoke
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---