---
swagger: "2.0"
x-collection-name: AWS Security Token Service
x-complete: 0
info:
  title: AWS Security Token Service API Get Session Token
  version: 1.0.0
  description: Returns a set of temporary credentials for an AWS account or IAM user.
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
  /?Action=GetSessionToken:
    get:
      summary: Get Session Token
      description: Returns a set of temporary credentials for an AWS account or IAM
        user.
      operationId: getSessionToken
      x-api-path-slug: actiongetsessiontoken-get
      parameters:
      - in: query
        name: DurationSeconds
        description: The duration, in seconds, that the credentials should remain
          valid
        type: string
      - in: query
        name: SerialNumber
        description: The identification number of the MFA device that is associated
          with the IAM user who      is making the GetSessionToken call
        type: string
      - in: query
        name: TokenCode
        description: The value provided by the MFA device, if MFA is required
        type: string
      responses:
        200:
          description: OK
      tags:
      - Session Token
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