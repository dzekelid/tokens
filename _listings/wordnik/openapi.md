---
swagger: "2.0"
x-collection-name: Wordnik
x-complete: 1
info:
  title: Wordnik
  description: wordnik-is-the-worlds-biggest-online-english-dictionary-by-number-of-words
  version: "4.0"
host: api.wordnik.com
basePath: /v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account.json/apiTokenStatus:
    get:
      summary: Returns usage statistics for the API account.
      description: Returns usage statistics for the api account..
      operationId: getApiTokenStatus
      x-api-path-slug: account-jsonapitokenstatus-get
      parameters:
      - in: header
        name: api_key
        description: Wordnik authentication token
      responses:
        200:
          description: OK
      tags:
      - Account
      - ApiTokenStatus
---