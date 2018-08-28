---
swagger: "2.0"
x-collection-name: PredictHQ
x-complete: 0
info:
  title: PredictHQ Requesting an Access Token
  description: |-
    When requesting an Access Token, use the `client_credentials` grant type, then request the scope or scopes you wish to have access to.

    These scopes can be any or all of the following, separated by a space:
      - `account` Grants access to the account endpoint.
      - `events` Grants access to the events endpoint.
      - `places` Grants access to the places endpoint.
      - `signals` Grants access to the signals endpoint.

    Please note that Access Tokens requested via the client_credentials grant type never expire.
  version: 1.0.0
host: api.predicthq.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /oauth2/token/:
    post:
      summary: Requesting an Access Token
      description: |-
        When requesting an Access Token, use the `client_credentials` grant type, then request the scope or scopes you wish to have access to.

        These scopes can be any or all of the following, separated by a space:
          - `account` Grants access to the account endpoint.
          - `events` Grants access to the events endpoint.
          - `places` Grants access to the places endpoint.
          - `signals` Grants access to the signals endpoint.

        Please note that Access Tokens requested via the client_credentials grant type never expire.
      operationId: Oauth2TokenPost
      x-api-path-slug: oauth2token-post
      parameters:
      - in: formData
        name: grant_type
      - in: formData
        name: scope
      responses:
        200:
          description: OK
      tags:
      - Oauth2
      - Token
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