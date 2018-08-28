swagger: "2.0"
x-collection-name: Google Play
x-complete: 1
info:
  title: Google Play
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /enterprises/{enterpriseId}/createWebToken:
    post:
      summary: Create Web Token
      description: Returns a unique token to access an embeddable UI. To generate
        a web UI, pass the generated token into the managed Google Play javascript
        API. Each token may only be used to start one UI session. See the javascript
        API documentation for further information.
      operationId: androidenterprise.enterprises.createWebToken
      x-api-path-slug: enterprisesenterpriseidcreatewebtoken-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      responses:
        200:
          description: OK
      tags:
      - Token
  /enterprises/{enterpriseId}/users/{userId}/authenticationToken:
    post:
      summary: Generate Authentication Token
      description: |-
        Generates an authentication token which the device policy client can use to provision the given EMM-managed user account on a device. The generated token is single-use and expires after a few minutes.

        This call only works with EMM-managed accounts.
      operationId: androidenterprise.users.generateAuthenticationToken
      x-api-path-slug: enterprisesenterpriseidusersuseridauthenticationtoken-post
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Token
  /enterprises/{enterpriseId}/users/{userId}/token:
    delete:
      summary: Delete User Token
      description: Revokes a previously generated token (activation code) for the
        user.
      operationId: androidenterprise.users.revokeToken
      x-api-path-slug: enterprisesenterpriseidusersuseridtoken-delete
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Token
    post:
      summary: Generate User Token
      description: |-
        Generates a token (activation code) to allow this user to configure their managed account in the Android Setup Wizard. Revokes any previously generated token.

        This call only works with Google managed accounts.
      operationId: androidenterprise.users.generateToken
      x-api-path-slug: enterprisesenterpriseidusersuseridtoken-post
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - Token
  /applications/{applicationId}/verify:
    get:
      summary: Verify Token
      description: Verifies the auth token provided with this request is for the application
        with the specified ID, and returns the ID of the player it was granted for.
      operationId: games.applications.verify
      x-api-path-slug: applicationsapplicationidverify-get
      parameters:
      - in: path
        name: applicationId
        description: The application ID from the Google Play developer console
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      responses:
        200:
          description: OK
      tags:
      - Token
  /pushtokens:
    put:
      summary: Register Push Token
      description: Registers a push token for the current user and application.
      operationId: games.pushtokens.update
      x-api-path-slug: pushtokens-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      responses:
        200:
          description: OK
      tags:
      - Token
  /pushtokens/remove:
    post:
      summary: Remove Push Token
      description: Removes a push token for the current user and application. Removing
        a non-existent push token will report success.
      operationId: games.pushtokens.remove
      x-api-path-slug: pushtokensremove-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      responses:
        200:
          description: OK
      tags:
      - Token