---
swagger: "2.0"
x-collection-name: Respoke
x-complete: 0
info:
  title: Respoke REST API Tokens
  description: By using the App-Secret header, you can perform API calls to obtain
    Respoke sessions for your users via POST to [base]/tokens. App-Secrets are found
    in the Dev Console.
  termsOfService: https://www.respoke.io/files/respoke-tos-20141007.pdf
  version: v1
host: api.respoke.io
basePath: v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  session-tokens/:
    post:
      summary: Session Tokens
      description: An end-user client posts a tokenId from POST [base]/tokens to authenticate
        to an app as endpointId.
      operationId: postSessionTokens
      x-api-path-slug: sessiontokens-post
      parameters:
      - schema:
          $ref: '#/definitions/holder'
      - in: header
        name: App-Token
        description: Your application token
      responses:
        200:
          description: OK
      tags:
      - Session
      - Tokens
  tokens/:
    post:
      summary: Tokens
      description: Get an access token tokenId for an end-user.
      operationId: postTokens
      x-api-path-slug: tokens-post
      parameters:
      - schema:
          $ref: '#/definitions/holder'
      - in: header
        name: App-Secret
        description: Your application secret
      responses:
        200:
          description: OK
      tags:
      - Tokens
    put:
      summary: Tokens
      description: By using the App-Secret header, you can perform API calls to obtain
        Respoke sessions for your users via POST to [base]/tokens. App-Secrets are
        found in the Dev Console.
      operationId: putTokens
      x-api-path-slug: tokens-put
      parameters:
      - in: query
        name: App-Secret
        description: Your application token
      responses:
        200:
          description: OK
      tags:
      - Tokens
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