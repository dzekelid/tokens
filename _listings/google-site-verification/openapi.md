swagger: "2.0"
x-collection-name: Google Site Verification
x-complete: 1
info:
  title: Google Site Verification
  description: verifies-ownership-of-websites-or-domains-with-google-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /siteVerification/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /token:
    post:
      summary: Get Token
      description: Get a verification token for placing on a website or domain.
      operationId: siteVerification.webResource.getToken
      x-api-path-slug: token-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Token