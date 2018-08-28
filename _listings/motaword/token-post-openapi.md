---
swagger: "2.0"
x-collection-name: MotaWord
x-complete: 0
info:
  title: Mota Word Retrieve an access token to interact with the API.
  description: MotaWord API is using OAuth2 procedures when authenticating or authorizing
    your API call. Currently, we only allow Client Credential type flow.
  version: alpha-0.1.0
host: api.motaword.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /token:
    post:
      summary: Retrieve an access token to interact with the API.
      description: MotaWord API is using OAuth2 procedures when authenticating or
        authorizing your API call. Currently, we only allow Client Credential type
        flow.
      operationId: getAccessToken
      x-api-path-slug: token-post
      parameters:
      - in: header
        name: Authorization
        description: HTTP Basic Authorization header
      - in: formData
        name: grant_type
        description: OAuth2 grant type
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