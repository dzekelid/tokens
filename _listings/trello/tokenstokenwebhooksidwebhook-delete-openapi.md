---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Delete Tokens Webhooks
  description: Delete tokens webhooks.
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /members/{idMember}/tokens:
    get:
      summary: Get Members Tokens
      description: Get members tokens.
      operationId: getMembersTokensByIdMember
      x-api-path-slug: membersidmembertokens-get
      parameters:
      - in: query
        name: filter
        description: 'One of: all or none'
      - in: path
        name: idMember
        description: idMember or username
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Members
      - Tokens
  /tokens/{token}:
    delete:
      summary: Delete Tokens
      description: Delete tokens.
      operationId: deleteTokensByToken
      x-api-path-slug: tokenstoken-delete
      parameters:
      - in: query
        name: key
        description: Generate your application key
      - in: path
        name: token
        description: token
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Tokens
    get:
      summary: Get Tokens
      description: Get tokens.
      operationId: getTokensByToken
      x-api-path-slug: tokenstoken-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: dateCreated, dateExpires,
          idMember, identifier or permissions'
      - in: query
        name: key
        description: Generate your application key
      - in: path
        name: token
        description: token
      - in: query
        name: token
        description: Getting a token from a user
      - in: query
        name: webhooks
        description: true or false
      responses:
        200:
          description: OK
      tags:
      - Tokens
  /tokens/{token}/member:
    get:
      summary: Get Tokens Member
      description: Get tokens member.
      operationId: getTokensMemberByToken
      x-api-path-slug: tokenstokenmember-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: avatarHash, avatarSource,
          bio, bioData, confirmed, email, fullName, gravatarHash, idBoards, idBoardsPinned,
          idOrganizations, idPremOrgsAdmin, initials, loginTypes, memberType, oneTimeMessagesDismissed,
          prefs, premiumFeatures, products, status, status, trophies, uploadedAvatarHash,
          url or username'
      - in: query
        name: key
        description: Generate your application key
      - in: path
        name: token
        description: token
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Tokens
      - Member
  /tokens/{token}/member/{field}:
    get:
      summary: Get Tokens Member Field
      description: Get tokens member field.
      operationId: getTokensMemberByTokenByField
      x-api-path-slug: tokenstokenmemberfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: query
        name: key
        description: Generate your application key
      - in: path
        name: token
        description: token
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Tokens
      - Member
      - Field
  /tokens/{token}/webhooks:
    get:
      summary: Get Tokens Webhooks
      description: Get tokens webhooks.
      operationId: getTokensWebhooksByToken
      x-api-path-slug: tokenstokenwebhooks-get
      parameters:
      - in: query
        name: key
        description: Generate your application key
      - in: path
        name: token
        description: token
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Tokens
      - Webhooks
    post:
      summary: Post Tokens Webhooks
      description: Post tokens webhooks.
      operationId: addTokensWebhooksByToken
      x-api-path-slug: tokenstokenwebhooks-post
      parameters:
      - in: body
        name: body
        description: Attributes of Tokens Webhooks to be added
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: key
        description: Generate your application key
      - in: path
        name: token
        description: token
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Tokens
      - Webhooks
    put:
      summary: Put Tokens Webhooks
      description: Put tokens webhooks.
      operationId: updateTokensWebhooksByToken
      x-api-path-slug: tokenstokenwebhooks-put
      parameters:
      - in: body
        name: body
        description: Attributes of Tokens Webhooks to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: key
        description: Generate your application key
      - in: path
        name: token
        description: token
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Tokens
      - Webhooks
  /tokens/{token}/webhooks/{idWebhook}:
    delete:
      summary: Delete Tokens Webhooks
      description: Delete tokens webhooks.
      operationId: deleteTokensWebhooksByTokenByIdWebhook
      x-api-path-slug: tokenstokenwebhooksidwebhook-delete
      parameters:
      - in: path
        name: idWebhook
        description: idWebhook
      - in: query
        name: key
        description: Generate your application key
      - in: path
        name: token
        description: token
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Tokens
      - Webhooks
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