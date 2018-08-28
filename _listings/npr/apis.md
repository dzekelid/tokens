---
name: NPR
x-slug: npr
description: NPR delivers breaking national and world news. Also top stories from
  business, politics, health, science, technology, music, arts and culture. Subscribe
  to podcasts and RSS feeds.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/141-npr.jpg
x-kinRank: "9"
x-alexaRank: "598"
tags: Tokens
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/npr/apis.md
specificationVersion: "0.14"
apis:
- name: NPR One API Reference - Create a new OAuth2 access token
  x-api-slug: authorizationv2token-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/141-npr.jpg
  humanURL: http://npr.org
  baseURL: https://api.npr.org//
  tags: News, Radio, Getting Started Example, Federal Government, Stack Network, Stack,
    Mobile, Media, API Provider, Broadcasts, Profiles, Publish, General Data, Relative
    Data, Service API, Pedestal, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/npr/authorizationv2token-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/npr/authorizationv2token-post-openapi.md
- name: NPR One API Reference - Revoke an existing OAuth2 access token
  x-api-slug: authorizationv2tokenrevoke-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/141-npr.jpg
  humanURL: http://npr.org
  baseURL: https://api.npr.org//
  tags: News, Radio, Getting Started Example, Federal Government, Stack Network, Stack,
    Mobile, Media, API Provider, Broadcasts, Profiles, Publish, General Data, Relative
    Data, Service API, Pedestal, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/npr/authorizationv2tokenrevoke-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/npr/authorizationv2tokenrevoke-post-openapi.md
- name: NPR One API Reference - Revoke an existing OAuth2 access token
  x-api-slug: authorizationv2tokenrevoke-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/141-npr.jpg
  humanURL: http://npr.org
  baseURL: https://api.npr.org//
  tags: News, Radio, Getting Started Example, Federal Government, Stack Network, Stack,
    Mobile, Media, API Provider, Broadcasts, Profiles, Publish, General Data, Relative
    Data, Service API, Pedestal, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/npr/authorizationv2tokenrevoke-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/npr/authorizationv2tokenrevoke-post-openapi.md
- name: NPR One API Reference - Create a new OAuth2 access token
  x-api-slug: authorizationv2token-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/141-npr.jpg
  humanURL: http://npr.org
  baseURL: https://api.npr.org//
  tags: News, Radio, Getting Started Example, Federal Government, Stack Network, Stack,
    Mobile, Media, API Provider, Broadcasts, Profiles, Publish, General Data, Relative
    Data, Service API, Pedestal, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/npr/authorizationv2token-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/npr/authorizationv2token-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://nfusion.solutions.api.gallery.streamdata.io
- type: x-api-stack
  url: http://npr.stack.network
- type: x-base
  url: http://api.npr.org/
- type: x-codecademy
  url: http://www.codecademy.com/tracks/npr
- type: x-crunchbase
  url: https://crunchbase.com/organization/npr
- type: x-crunchbase
  url: http://www.crunchbase.com/company/npr
- type: x-developer
  url: http://dev.npr.org/
- type: x-documentation
  url: http://dev.npr.org/#accessing-the-api
- type: x-email
  url: permissions@npr.org
- type: x-email
  url: ogcstaff@npr.org
- type: x-email
  url: employment@npr.org
- type: x-email
  url: careers@npr.org
- type: x-email
  url: kroc@npr.org
- type: x-email
  url: mediarelations@npr.org
- type: x-email
  url: sponsorship@npr.org
- type: x-email
  url: ashamblin@npr.org
- type: x-email
  url: giving@npr.org
- type: x-email
  url: giftplanning@npr.org
- type: x-email
  url: NPRDonorCommunications@npr.org
- type: x-getting-started
  url: http://dev.npr.org/#quick-start
- type: x-github
  url: https://github.com/npr
- type: x-selfservice-registration
  url: http://www.npr.org/templates/reg/
- type: x-terms-of-service
  url: http://www.npr.org/about-npr/179876898/terms-of-use
- type: x-twitter
  url: https://twitter.com/NPR
- type: x-twitter
  url: https://twitter.com/NPRTechTeam
- type: x-website
  url: http://npr.org
- type: x-website
  url: http://www.npr.org
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---