---
swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 0
info:
  title: Urban Airship Get Device Tokens Count
  description: Gets the number of device tokens you have registered.
  version: v3
host: go.urbanairship.com
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /device_tokens/{token}:
    put:
      summary: Put Device Tokens Token
      description: Registers a device token.
      operationId: device_tokens.token.put
      x-api-path-slug: device-tokenstoken-put
      parameters:
      - in: query
        name: token
        description: Device tokens should be represented as an uppercase string, 64
          characters long, without spaces or other separators
      - in: path
        name: token
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Token
    get:
      summary: Get Device Tokens Token
      description: Gets a device token???s alias.
      operationId: device_tokens.token.get
      x-api-path-slug: device-tokenstoken-get
      parameters:
      - in: query
        name: token
        description: Device tokens should be represented as an uppercase string, 64
          characters long, without spaces or other separators
      - in: path
        name: token
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Token
    delete:
      summary: Delete Device Tokens Token
      description: Marks the device token as inactive. No notifications will be delivered
        to it until a PUT is executed again. The DELETE returns HTTP 204 No Content,
        and needs no payload. When a token is deleted in this manner, any alias or
        tags will be cleared.
      operationId: device_tokens.token.delete
      x-api-path-slug: device-tokenstoken-delete
      parameters:
      - in: query
        name: token
        description: Device tokens should be represented as an uppercase string, 64
          characters long, without spaces or other separators
      - in: path
        name: token
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Token
  /device_tokens:
    get:
      summary: Get Device Tokens
      description: Gets information about all of your device tokens. If your application
        has a large number of device tokens, we???ll paginate the request for you.
        By default, we paginate at 5000 device tokens. You can receive the next page
        simply by retrieving the URL from "next_page" - in this way it is easy to
        export all of your device tokens and all their data.
      operationId: device_tokens.get
      x-api-path-slug: device-tokens-get
      parameters:
      - in: query
        name: limit
        description: The total items to return
      - in: query
        name: page
        description: The page number
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
  /device_tokens/count:
    get:
      summary: Get Device Tokens Count
      description: Gets the number of device tokens you have registered.
      operationId: device_tokens.count.get
      x-api-path-slug: device-tokenscount-get
      parameters:
      - in: query
        name: limit
        description: The total items to return
      - in: query
        name: page
        description: The page number
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Count
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