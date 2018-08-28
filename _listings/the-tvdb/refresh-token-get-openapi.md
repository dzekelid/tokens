---
swagger: "2.0"
x-collection-name: The TVDB
x-complete: 0
info:
  title: The TVDB Get Refresh Token
  description: Refreshes your current, valid JWT token and returns a new token. Hit
    this route so that you do not have to post to `/login` with your API key and credentials
    once you have already been authenticated.
  version: 2.1.2
host: api-dev.thetvdb.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /refresh_token:
    get:
      summary: Get Refresh Token
      description: Refreshes your current, valid JWT token and returns a new token.
        Hit this route so that you do not have to post to `/login` with your API key
        and credentials once you have already been authenticated.
      operationId: refresh_token.get
      x-api-path-slug: refresh-token-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - Refresh
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