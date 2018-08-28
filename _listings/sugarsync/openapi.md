swagger: "2.0"
x-collection-name: SugarSync
x-complete: 1
info:
  title: SugarSync  API
  description: the-sugarsync-service-presents-a-set-of-resources-that-your-application-can-access-through-the-platform-api--
  version: "1"
host: api.sugarsync.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /app-authorization:
    post:
      summary: Creating a Refresh Token
      description: An application needs to be authorized to access a users SugarSync
        resources through the Platform API.nTo do that, the app needs to create a
        refresh token. When a user first runs the application, it creates a refresh
        tokennby submitting a POST request that includes the users credentials to
        the API.nIf the request is successful, the SugarSync service grants the application
        permission to access the users account and returns a refresh token.n
      operationId: creating-a-refresh-token
      x-api-path-slug: appauthorization-post
      parameters:
      - in: header
        name: Content-Length
        description: The length of the request body
      - in: header
        name: Content-Type
        description: The content type and character encoding of the response
      - in: header
        name: Host
        description: The domain name of the server
      - in: header
        name: User-Agent
        description: The client application implementing the network protocol for
          communication between          the client and server
      responses:
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
        200:
          description: OK
      tags:
      - App
      - Authorization