---
swagger: "2.0"
x-collection-name: NetLicensing
x-complete: 0
info:
  title: NetLicensing Create token
  description: Create token by tokenType and additional token parameters
  termsOfService: https://www.labs64.com/legal/terms-of-service/netlicensing
  version: 2.x
host: go.netlicensing.io
basePath: /core/v2/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /token/{tokenNumber}:
    delete:
      summary: Delete token
      description: Delete a token by number
      operationId: deleteToken
      x-api-path-slug: tokentokennumber-delete
      parameters:
      - in: path
        name: tokenNumber
        description: Token number
      responses:
        200:
          description: OK
      tags:
      - Token
      - TokenNumber
    get:
      summary: Get token
      description: Return a token by tokenNumber
      operationId: getToken
      x-api-path-slug: tokentokennumber-get
      parameters:
      - in: path
        name: tokenNumber
        description: Token number
      responses:
        200:
          description: OK
      tags:
      - Token
      - TokenNumber
  /token:
    get:
      summary: Tokens list
      description: Return a list of all tokens for the current vendor
      operationId: listTokens
      x-api-path-slug: token-get
      responses:
        200:
          description: OK
      tags:
      - Token
    post:
      summary: Create token
      description: Create token by tokenType and additional token parameters
      operationId: createToken
      x-api-path-slug: token-post
      parameters:
      - in: formData
        name: cancelURL
        description: for tokenType=SHOP only; take customers to this URL when they
          cancel their checkout
      - in: formData
        name: cancelURLTitle
        description: for tokenType=SHOP only; shop link title for cancel checkout
          process
      - in: formData
        name: licenseeNumber
        description: for tokenType=SHOP only (mandatory); identifies licensee that
          will be assigned to the shop token
      - in: formData
        name: successURL
        description: for tokenType=SHOP only; take customers to this URL when they
          finish checkout
      - in: formData
        name: successURLTitle
        description: for tokenType=SHOP only; shop link title for successful checkout
          process
      - in: formData
        name: tokenType
        description: Token type to be generated
      responses:
        200:
          description: OK
      tags:
      - Token
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