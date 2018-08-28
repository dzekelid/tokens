swagger: "2.0"
x-collection-name: Rebilly
x-complete: 1
info:
  title: Rebilly
  description: -introductionthe-rebilly-api-is-built-on-http---our-api-is-restful---it-has-predictableresource-urls---it-returns-http-response-codes-to-indicate-errors---it-alsoaccepts-and-returns-json-in-the-http-body---you-can-use-your-favoritehttprest-library-for-your-programming-language-to-use-rebillys-api-oryou-can-use-one-of-our-sdks-currently-available-in-phphttpsgithub-comrebillyrebillyphpand-chttpsgithub-comrebillyrebillydotnetclient--authenticationwhen-you-sign-up-for-an-account-you-are-given-your-first-api-key-you-can-generate-additional-api-keys-and-delete-api-keys-as-you-mayneed-to-rotate-your-keys-in-the-future--you-authenticate-to-therebilly-api-by-providing-your-secret-key-in-the-request-header-rebilly-offers-three-forms-of-authentication--private-key-json-web-tokens-andpublic-key--private-key-authenticates-each-request-by-searching-for-the-presenceof-an-http-header-rebapikey--jwt-authenticates-each-request-by-the-http-header-authorization--public-key-authenticates-by-the-http-header-rebauth-read-more-on-this-below-rebilly-also-offers-json-web-tokens-jwt-authentication-where-you-can-controlthe-specific-granular-permissions-and-expiration-for-that-jwt---we-call-our-resourcefor-generating-jwt-sessionstagsessions-rebilly-also-has-a-clientside-authentication-scheme-that-uses-anapiuser-and-hmacsha1-signature-only-for-the-tokens-resource-sothat-you-may-safely-create-tokens-from-the-clientside-without-compromisingyour-secret-keys-never-share-your-secret-keys--keep-them-guarded-and-secure-the-clientside-authentication-scheme-uses-one-http-header-named-rebauth--redocinject-securitydefinitions--php-sdkfor-all-php-sdk-examples-provided-in-this-spec-you-will-need-to-configure-client-you-may-do-it-like-thisphpclient--new-rebillyclient----apikey--yourapikeyhere----baseurl--httpsapi-rebilly-com
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /authentication-tokens:
    get:
      summary: Retrieve a list of auth tokens
      description: Retrieve a list of auth tokens
      operationId: authentication_tokens.get
      x-api-path-slug: authenticationtokens-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Auth
      - Tokens
  /password-tokens:
    get:
      summary: Retrieve a list of tokens
      description: Retrieve a list of tokens
      operationId: password_tokens.get
      x-api-path-slug: passwordtokens-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Tokens
    post:
      summary: Create a Reset Password Token
      description: Create a Reset Password Token
      operationId: password_tokens.post
      x-api-path-slug: passwordtokens-post
      parameters:
      - in: body
        name: body
        description: ResetPasswordToken resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Reset
      - Password
      - Token
  /tokens:
    get:
      summary: Retrieve a list of tokens
      description: Retrieve a list of tokens
      operationId: tokens.get
      x-api-path-slug: tokens-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Tokens
    post:
      summary: Create a payment token
      description: Create a token
      operationId: tokens.post
      x-api-path-slug: tokens-post
      parameters:
      - in: body
        name: body
        description: PaymentToken resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Token
  /password-tokens/{id}:
    delete:
      summary: Delete a Reset Password Token
      description: Delete a Reset Password Token with predefined identifier string
      operationId: password_tokens.id.delete
      x-api-path-slug: passwordtokensid-delete
      responses:
        200:
          description: OK
      tags:
      - Reset
      - Password
      - Token
    get:
      summary: Retrieve a Reset Password Token
      description: Retrieve a Reset Password Token with specified identifier string
      operationId: password_tokens.id.get
      x-api-path-slug: passwordtokensid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Reset
      - Password
      - Token
  /tokens/{token}:
    get:
      summary: Retrieve a token
      description: Retrieve a token with specified identifier string
      operationId: tokens.token.get
      x-api-path-slug: tokenstoken-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Token
  /tokens/{token}/expiration:
    post:
      summary: Expire a token
      description: Expire a token
      operationId: tokens.token.expiration.post
      x-api-path-slug: tokenstokenexpiration-post
      parameters:
      - in: body
        name: body
        description: PaymentToken resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Expire
      - Token
  /activation/{token}:
    post:
      summary: Sends a token to activate user account
      description: Sends a token to activate user account
      operationId: sends-a-token-to-activate-user-account
      x-api-path-slug: activationtoken-post
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Token
      - To
      - Activate
      - User
      - Account
  /forgot-password:
    post:
      summary: Sends an email with a link containing a token to reset user password
      description: Sends an email with a link containing a token to reset user password
      operationId: sends-an-email-with-a-link-containing-a-token-to-reset-user-password
      x-api-path-slug: forgotpassword-post
      parameters:
      - in: body
        name: body
        description: Email resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Email
      - Link
      - Containing
      - Token
      - To
      - Reset
      - User
      - Password