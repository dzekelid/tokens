swagger: "2.0"
x-collection-name: Digital River
x-complete: 1
info:
  title: Digital River Shopper API
  description: the-dr-connect-shopper-api-operates-on-a-store-and-products-that-are-set-up-in-global-commerce--
  version: v1
host: store.digitalriver.com
basePath: /store/{mysite}
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /oauth20/token:
    post:
      summary: Post Oauth20 Token
      description: Post oauth20 token.
      operationId: postOauth20Token
      x-api-path-slug: oauth20token-post
      responses:
        200:
          description: OK
      tags:
      - Oauth20
      - Token
  /v1/shoppers/token:
    get:
      summary: Get Shoppers Token
      description: Get shoppers token.
      operationId: getV1ShoppersToken
      x-api-path-slug: v1shopperstoken-get
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Token