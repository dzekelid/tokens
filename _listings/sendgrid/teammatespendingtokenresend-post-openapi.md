---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Add Teammates Pending Token Resend
  description: |-
    This endpoint allows you to resend a teammate invite.

    **Note:** Teammate invitations will expire after 7 days. Resending an invite will reset the expiration date.
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /teammates/pending/{token}:
    delete:
      summary: Delete Teammates Pending Token
      description: This endpoint allows you to delete a pending teammate invite.
      operationId: teammates.pending.token.delete
      x-api-path-slug: teammatespendingtoken-delete
      responses:
        200:
          description: OK
      tags:
      - Email
      - Teammates
      - Pending
      - Token
  /teammates/pending/{token}/resend:
    post:
      summary: Add Teammates Pending Token Resend
      description: |-
        This endpoint allows you to resend a teammate invite.

        **Note:** Teammate invitations will expire after 7 days. Resending an invite will reset the expiration date.
      operationId: teammates.pending.token.resend.post
      x-api-path-slug: teammatespendingtokenresend-post
      responses:
        200:
          description: OK
      tags:
      - Email
      - Teammates
      - Pending
      - Token
      - Resend
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