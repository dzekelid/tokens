swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/token/validate:
    post:
      summary: Validate the oauth2 token
      description: Validate the oauth2 token for the gateway usage
      operationId: validate-the-oauth2-token-for-the-gateway-usage
      x-api-path-slug: apitokenvalidate-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer *your_token
      - in: header
        name: Predix-Zone-Id
      responses:
        200:
          description: Successful response
      tags:
      - Validate
      - Oauth2
      - Token