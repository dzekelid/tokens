---
swagger: "2.0"
x-collection-name: AWS Security Token Service
x-complete: 0
info:
  title: AWS Security Token Service API Get Federation Token
  version: 1.0.0
  description: |-
    Returns a set of temporary security credentials (consisting of an access key ID, a
          secret access key, and a security token) for a federated user.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetFederationToken:
    get:
      summary: Get Federation Token
      description: |-
        Returns a set of temporary security credentials (consisting of an access key ID, a
              secret access key, and a security token) for a federated user.
      operationId: getFederationToken
      x-api-path-slug: actiongetfederationtoken-get
      parameters:
      - in: query
        name: DurationSeconds
        description: The duration, in seconds, that the session should last
        type: string
      - in: query
        name: Name
        description: The name of the federated user
        type: string
      - in: query
        name: Policy
        description: An IAM policy in JSON format that is passed with the GetFederationToken      call
          and evaluated along with the policy or policies that are attached to the
          IAM user whose      credentials are used to call GetFederationToken
        type: string
      responses:
        200:
          description: OK
      tags:
      - Federation Token
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