swagger: "2.0"
x-collection-name: MotaWord
x-complete: 1
info:
  title: Mota Word
  description: use-motaword-api-to-post-and-track-your-translation-projects-
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