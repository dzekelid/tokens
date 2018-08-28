swagger: "2.0"
x-collection-name: Actility
x-complete: 1
info:
  title: ThingPark DX Maker API
  description: api-providing-features-for-device-makers-such-as-preprovisioning-on-standalone-join-servers-
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /maker/v011/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /oauth/token:
    post:
      summary: Token Generation
      description: Generates and retrieves a token for a client.
      operationId: generates-and-retrieves-a-token-for-a-client
      x-api-path-slug: oauthtoken-post
      parameters:
      - in: formData
        name: client_id
        description: Id of the client
      - in: formData
        name: client_secret
        description: Secret of the client
      - in: formData
        name: grant_type
        description: Type of the OAuth2 grant workflow
      - in: query
        name: renewToken
        description: Forces the token to be renewed
      - in: query
        name: validityPeriod
        description: Validity of the new token
      responses:
        200:
          description: OK
      tags:
      - Token
      - Generation
  /oauth/revoke_token:
    post:
      summary: Token Revocation
      description: Revokes a token.
      operationId: revokes-a-token
      x-api-path-slug: oauthrevoke-token-post
      parameters:
      - in: query
        name: access_token
        description: Value of the token to revoke
      responses:
        200:
          description: OK
      tags:
      - Token
      - Revocation
  /oauth/tokeninfo:
    get:
      summary: Token Info Retrieval
      description: Retrieves information about a valid token.
      operationId: retrieves-information-about-a-valid-token
      x-api-path-slug: oauthtokeninfo-get
      parameters:
      - in: query
        name: access_token
        description: Value of the token for which info is requested
      responses:
        200:
          description: OK
      tags:
      - Token
      - Info
      - Retrieval