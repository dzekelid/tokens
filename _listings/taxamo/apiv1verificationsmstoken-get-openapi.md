---
swagger: "2.0"
x-collection-name: Taxamo
x-complete: 0
info:
  title: Taxamo Verify SMS Token
  description: Verify sms token.
  version: "1"
host: api.taxamo.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/verification/sms:
    post:
      summary: Create SMS Token
      description: Create sms token.
      operationId: createSMSToken
      x-api-path-slug: apiv1verificationsms-post
      parameters:
      - in: body
        name: input
        description: Input
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - SMS
      - Token
  /api/v1/verification/sms/{token}:
    get:
      summary: Verify SMS Token
      description: Verify sms token.
      operationId: verifySMSToken
      x-api-path-slug: apiv1verificationsmstoken-get
      parameters:
      - in: path
        name: token
        description: Provided token
      responses:
        200:
          description: OK
      tags:
      - Verify
      - SMS
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