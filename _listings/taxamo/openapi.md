swagger: "2.0"
x-collection-name: Taxamo
x-complete: 1
info:
  title: Taxamo
  description: taxamos-elegant-suite-of-apis-and-comprehensive-reporting-dashboard-enables-digital-merchants-to-easily-comply-with-eu-regulatory-requirements-on-tax-calculation-evidence-collection-tax-return-creation-and-data-storage-
  version: "1"
host: api.taxamo.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/verification/sms:
    post:
      summary: Create SMS Token
      description: Create sms token.
      operationId: createSMSToken
      x-api-path-slug: apiv1verificationsms-post
      parameters:
      - in: body
        name: input
        description: Input
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - SMS
      - Token
  /api/v1/verification/sms/{token}:
    get:
      summary: Verify SMS Token
      description: Verify sms token.
      operationId: verifySMSToken
      x-api-path-slug: apiv1verificationsmstoken-get
      parameters:
      - in: path
        name: token
        description: Provided token
      responses:
        200:
          description: OK
      tags:
      - Verify
      - SMS
      - Token