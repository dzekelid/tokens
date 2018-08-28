---
swagger: "2.0"
x-collection-name: 123FormBuilder
x-complete: 0
info:
  title: 123FormBuilder Invalidate token
  version: 1.0.0
  description: Invalidate token
host: api.123contactform.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /token/refresh:
    post:
      summary: Refresh token
      description: Refresh token
      operationId: refresh-token
      x-api-path-slug: tokenrefresh-post
      parameters:
      - in: formData
        name: JWT
        description: JWT authentication token
      responses:
        200:
          description: OK
      tags:
      - Refresh
      - Token
  /token/invalidate:
    post:
      summary: Invalidate token
      description: Invalidate token
      operationId: invalidate-token
      x-api-path-slug: tokeninvalidate-post
      parameters:
      - in: formData
        name: JWT
        description: JWT authentication token
      responses:
        200:
          description: OK
      tags:
      - Invalidate
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