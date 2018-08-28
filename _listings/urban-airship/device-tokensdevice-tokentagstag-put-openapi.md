---
swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 0
info:
  title: Urban Airship Put Device Tokens Device Token Tags Tag
  description: Creates a tag and associate it with the specific device token.
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
  /device_tokens/feedback:
    get:
      summary: Get Device Tokens Feedback
      description: Gets what device tokens are now invalid. Apple informs us when
        a push notification is sent to a device that can???t receive it because the
        application has been uninstalled. We mark the device token as inactive and
        immediately stop sending notifications to that device. Once a day is a good
        interval for querying the feedback service, but you can do it more often to
        save on bandwidth from unnecessary notifications. In the response, what does
        marked_inactive_on mean? Apple sends a timestamp for each device token returned
        via the feedback service. Since a device can be off the network for a while,
        this can be a point in the recent past. In order to make this API work smoothly
        for you, we record the timestamp we marked as inactive. This means you only
        need to query for data since the last time you queried. Once a day is a good
        timeframe, or once a week for very small or infrequently used applications.
        A few times a day is good for applications with heavy use.
      operationId: device_tokens.feedback.get
      x-api-path-slug: device-tokensfeedback-get
      parameters:
      - in: query
        name: since
        description: Since timestamp in ISO 8601 format
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Feedback
  /device_tokens/{device_token}/tags:
    get:
      summary: Get Device Tokens Device Token Tags
      description: Gets tags for a specific device token.
      operationId: device_tokens.device_token.tags.get
      x-api-path-slug: device-tokensdevice-tokentags-get
      parameters:
      - in: query
        name: device_token
        description: A specific device token
      - in: path
        name: device_token
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Device
      - Token
      - Tags
  /device_tokens/{device_token}/tags/{tag}:
    put:
      summary: Put Device Tokens Device Token Tags Tag
      description: Creates a tag and associate it with the specific device token.
      operationId: device_tokens.device_token.tags.tag.put
      x-api-path-slug: device-tokensdevice-tokentagstag-put
      parameters:
      - in: query
        name: device_token
        description: A specific device token
      - in: path
        name: device_token
      - in: query
        name: tag
        description: Tags can be of any format you wish, but we recommend that they
          be URL-safe in order to make less work for you
      - in: path
        name: tag
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Device
      - Token
      - Tags
      - Tag
    delete:
      summary: Delete Device Tokens Device Token Tags Tag
      description: Removes a single tag from a device token.
      operationId: device_tokens.device_token.tags.tag.delete
      x-api-path-slug: device-tokensdevice-tokentagstag-delete
      parameters:
      - in: query
        name: device_token
        description: A specific device token
      - in: path
        name: device_token
      - in: query
        name: tag
        description: Tags can be of any format you wish, but we recommend that they
          be URL-safe in order to make less work for you
      - in: path
        name: tag
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Device
      - Token
      - Tags
      - Tag
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