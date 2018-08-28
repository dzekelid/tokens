swagger: "2.0"
x-collection-name: 123FormBuilder
x-complete: 1
info:
  title: ""
  version: 1.0.0
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