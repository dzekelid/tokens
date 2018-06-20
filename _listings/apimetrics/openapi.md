---
swagger: "2.0"
x-collection-name: APImetrics
x-complete: 1
info:
  title: APImetrics Merged API
  version: 1.0.0
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
    put:
      summary: Update an Auth Token
      description: Update an Auth Token
      operationId: updateAnAuthToken
      x-api-path-slug: tokensid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID string of Token you are updating
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Tokens
---