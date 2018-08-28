---
swagger: "2.0"
x-collection-name: Docsmore
x-complete: 0
info:
  title: Docsmore Get OAuth TOKEN
  description: |-
    Obtaining an Auth Token is the first thing in the process. The lifetime of Auth token is configurable in the developer portal depending upon your need. Once auth token is obtained, all the follow up API calls will need to include auth token in the header. FaIlure to do so would result in response with 401 Unauthorized Access.

    Under Your Developer Account - Go to Api Setting and you will screen similar to below.


    Make sure you call this in server side code. Exposing apiKey and clientSecret is a not a good idea on front end and can lead up to security vulnerabilities.
  version: "1.0"
host: api.docsmore.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/clientdocs/getrawdata/:authToken/:documentKey:
    get:
      summary: Get Raw Data For A Given Document
      description: |-
        This API call gets you underlying raw data of the document. All you need to do is supply Auth token and Document Key as part of the call.

        Document Key can be obtained from "Document Gallery" Page and Clicking on the sub-menu of the desired document.

        As a response object, jsondata and metadata information is passed. Jsondata is basically raw data and metadata is data columns information.
      operationId: ApiClientdocsGetrawdataAuthTokenDocumentKeyGet
      x-api-path-slug: apiclientdocsgetrawdataauthtokendocumentkey-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: authToken
      - in: header
        name: Content-Type
      - in: query
        name: documentKey
      responses:
        200:
          description: OK
      tags:
      - Raw
      - Data
      - Given
      - Document
  /oauth/token:
    post:
      summary: Get OAuth TOKEN
      description: |-
        Obtaining an Auth Token is the first thing in the process. The lifetime of Auth token is configurable in the developer portal depending upon your need. Once auth token is obtained, all the follow up API calls will need to include auth token in the header. FaIlure to do so would result in response with 401 Unauthorized Access.

        Under Your Developer Account - Go to Api Setting and you will screen similar to below.


        Make sure you call this in server side code. Exposing apiKey and clientSecret is a not a good idea on front end and can lead up to security vulnerabilities.
      operationId: OauthTokenPost
      x-api-path-slug: oauthtoken-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - OAuth
      - TOKEN
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