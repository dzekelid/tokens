---
swagger: "2.0"
x-collection-name: APImetrics
x-complete: 0
info:
  title: APIMetrics Create a new Auth Token
  version: 1.0.0
  description: Create a new Auth Token
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