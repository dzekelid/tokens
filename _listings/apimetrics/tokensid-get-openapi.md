---
swagger: "2.0"
x-collection-name: APImetrics
x-complete: 0
info:
  title: APIMetrics Get an existing Auth Token
  version: 1.0.0
  description: Get an existing Auth Token
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tokens/:
    get:
      summary: List Auth Tokens
      description: List Auth Tokens
      operationId: listAuthTokens
      x-api-path-slug: tokens-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Tokens
    post:
      summary: Create a new Auth Token
      description: Create a new Auth Token
      operationId: createANewAuthToken
      x-api-path-slug: tokens-post
      parameters:
      - in: body
        name: body
        description: '{     meta: {         auth_id: agxkZXZ-dmlhdGVzdHNyGgsSDVNlcnZpY2VDb25maWcYgICAgKDLmgsM,         name:
          Minimal token name     } }'
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Tokens
  /tokens/auth/{auth_id}/:
    get:
      summary: Get all tokens for an Authentication Setting
      description: Get all tokens for an Authentication Setting
      operationId: getAllTokensForAnAuthenticationSetting
      x-api-path-slug: tokensauthauth-id-get
      parameters:
      - in: path
        name: auth_id
        description: ID of the Authentication Settings
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Tokens
      - Auth
      - Auth
  /tokens/{id}/:
    delete:
      summary: Delete an Auth Token
      description: Delete an Auth Token
      operationId: deleteAnAuthToken
      x-api-path-slug: tokensid-delete
      parameters:
      - in: path
        name: id
        description: ID string of Token you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Tokens
    get:
      summary: Get an existing Auth Token
      description: Get an existing Auth Token
      operationId: getAnExistingAuthToken
      x-api-path-slug: tokensid-get
      parameters:
      - in: path
        name: id
        description: ID string of Token you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
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