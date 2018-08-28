---
swagger: "2.0"
x-collection-name: AWS EC2 Container Registry Service
x-complete: 0
info:
  title: AWS EC2 Container Registry API Get Authorization Token
  version: 1.0.0
  description: Retrieves a token that is valid for a specified registry for 12 hours.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetAuthorizationToken:
    get:
      summary: Get Authorization Token
      description: Retrieves a token that is valid for a specified registry for 12
        hours.
      operationId: getAuthorizationToken
      x-api-path-slug: actiongetauthorizationtoken-get
      parameters:
      - in: query
        name: registryIds
        description: A list of AWS account IDs that are associated with the registries
          for which to get authorization tokens
        type: string
      responses:
        200:
          description: OK
      tags:
      - Authorization Tokens
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