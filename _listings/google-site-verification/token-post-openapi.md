---
swagger: "2.0"
x-collection-name: Google Site Verification
x-complete: 0
info:
  title: Google Site Verification API Get Token
  description: Get a verification token for placing on a website or domain.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /siteVerification/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /token:
    post:
      summary: Get Token
      description: Get a verification token for placing on a website or domain.
      operationId: siteVerification.webResource.getToken
      x-api-path-slug: token-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
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