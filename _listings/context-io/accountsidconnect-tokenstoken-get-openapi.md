---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 0
info:
  title: Context.IO Get Accounts Connect Tokens Token
  description: Gets information about a given connect token.
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /connect_tokens:
    get:
      summary: Get Connect Tokens
      description: Lists connect tokens created with your API key.
      operationId: listConnectTokens_
      x-api-path-slug: connect-tokens-get
      responses:
        200:
          description: OK
      tags:
      - Connect
      - Tokens
    post:
      summary: Post Connect Tokens
      description: Obtains a new connect_token.
      operationId: Create_obtainNewConnectToken_
      x-api-path-slug: connect-tokens-post
      parameters:
      - in: query
        name: callback_url
        description: When the users mailbox is connected to your API key, the browser
          will call this url (GET)
      - in: query
        name: email
        description: The email address of the account to be added
      - in: query
        name: first_name
        description: First name of the account holder
      - in: query
        name: last_name
        description: Last name of the account holder
      - in: query
        name: service_level
        description: Sets the service level of the accounts source to be created
      responses:
        200:
          description: OK
      tags:
      - Connect
      - Tokens
  /connect_tokens/{token}:
    get:
      summary: Get Connect Tokens Token
      description: Gets information about a given connect token.
      operationId: getConnectToken_
      x-api-path-slug: connect-tokenstoken-get
      parameters:
      - in: path
        name: token
        description: The unique random token used for the graphical account creation
          process
      responses:
        200:
          description: OK
      tags:
      - Connect
      - Tokens
      - Token
    delete:
      summary: Delete Connect Tokens Token
      description: Removes a given connect token.
      operationId: removeConnectToken_
      x-api-path-slug: connect-tokenstoken-delete
      parameters:
      - in: path
        name: token
        description: The unique random token used for the graphical account creation
          process
      responses:
        200:
          description: OK
      tags:
      - Connect
      - Tokens
      - Token
  /accounts/{id}/connect_tokens:
    get:
      summary: Get Accounts Connect Tokens
      description: Lists connect tokens created for an account.
      operationId: listAccountConnectTokens_
      x-api-path-slug: accountsidconnect-tokens-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Connect
      - Tokens
    post:
      summary: Post Accounts Connect Tokens
      description: Obtains a new connect_token for a specific account.
      operationId: Create_obtainNewAccountConnectToken_
      x-api-path-slug: accountsidconnect-tokens-post
      parameters:
      - in: query
        name: callback_url
        description: When the users mailbox is connected to your API key, the browser
          will call this url (GET)
      - in: query
        name: email
        description: The email address of the account to be added
      - in: query
        name: first_name
        description: First name of the account holder
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: last_name
        description: Last name of the account holder
      - in: query
        name: service_level
        description: Sets the service level of the accounts source to be created
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Connect
      - Tokens
  /accounts/{id}/connect_tokens/{token}:
    get:
      summary: Get Accounts Connect Tokens Token
      description: Gets information about a given connect token.
      operationId: getAccountConnectToken_
      x-api-path-slug: accountsidconnect-tokenstoken-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: token
        description: The unique random token used to add a second source to an existing
          account
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Connect
      - Tokens
      - Token
    delete:
      summary: Delete Accounts Connect Tokens Token
      description: Remove a given connect token.
      operationId: removeAccountConnectToken_
      x-api-path-slug: accountsidconnect-tokenstoken-delete
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: token
        description: The unique random token used to add a second source to an existing
          account
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Connect
      - Tokens
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