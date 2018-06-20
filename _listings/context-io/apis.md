---
name: Context.IO
x-slug: context-io
description: Create simple email webhooks and code against a free, RESTful, IMAP API.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
x-kinRank: "9"
x-alexaRank: "569975"
tags: Tokens
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/context-io/apis.md
specificationVersion: "0.14"
apis:
- name: Context.IO Get Connect Tokens
  x-api-slug: context-io
  description: Lists connect tokens created with your API key.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///connect_tokens
  tags: Connect,Tokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/context-io/connect-tokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/context-io/connect-tokens-get-openapi.md
- name: Context.IO Post Connect Tokens
  x-api-slug: context-io
  description: Obtains a new connect_token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///connect_tokens
  tags: Connect,Tokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/context-io/connect-tokens-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/context-io/connect-tokens-post-openapi.md
- name: Context.IO Get Connect Tokens Token
  x-api-slug: context-io
  description: Gets information about a given connect token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///connect_tokens/{token}
  tags: Connect,Tokens,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/context-io/connect-tokenstoken-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/context-io/connect-tokenstoken-get-openapi.md
- name: Context.IO Delete Connect Tokens Token
  x-api-slug: context-io
  description: Removes a given connect token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///connect_tokens/{token}
  tags: Connect,Tokens,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/context-io/connect-tokenstoken-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/context-io/connect-tokenstoken-delete-openapi.md
- name: Context.IO Get Accounts Connect Tokens
  x-api-slug: context-io
  description: Lists connect tokens created for an account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/connect_tokens
  tags: Accounts,Connect,Tokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/context-io/accountsidconnect-tokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/context-io/accountsidconnect-tokens-get-openapi.md
- name: Context.IO Post Accounts Connect Tokens
  x-api-slug: context-io
  description: Obtains a new connect_token for a specific account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/connect_tokens
  tags: Accounts,Connect,Tokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/context-io/accountsidconnect-tokens-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/context-io/accountsidconnect-tokens-post-openapi.md
- name: Context.IO Get Accounts Connect Tokens Token
  x-api-slug: context-io
  description: Gets information about a given connect token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/connect_tokens/{token}
  tags: Accounts,Connect,Tokens,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/context-io/accountsidconnect-tokenstoken-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/context-io/accountsidconnect-tokenstoken-get-openapi.md
- name: Context.IO Delete Accounts Connect Tokens Token
  x-api-slug: context-io
  description: Remove a given connect token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0///accounts/{id}/connect_tokens/{token}
  tags: Accounts,Connect,Tokens,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/context-io/accountsidconnect-tokenstoken-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/context-io/accountsidconnect-tokenstoken-delete-openapi.md
- name: Context.IO
  x-api-slug: context-io
  description: Context.IO is the missing email API that makes it easy and fastto integrate
    your users email data in your application.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0/
  tags: Tokens
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/context-io/openapi.md
x-common:
- type: x-base
  url: https://api.context.io/
- type: x-blog
  url: http://blog.context.io/
- type: x-blog-rss
  url: http://blog.context.io/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/product/context-io
- type: x-crunchbase
  url: https://crunchbase.com/organization/context-io
- type: x-documentation
  url: http://context.io/docs/2.0
- type: x-email
  url: hello@context.io
- type: x-email
  url: support@context.io
- type: x-email
  url: business@context.io
- type: x-faq
  url: http://context.io/privacy-faq
- type: x-github
  url: https://github.com/contextio
- type: x-ios-library
  url: https://github.com/contextio/contextio-ios
- type: x-node-js-library
  url: https://github.com/contextio/ContextIO-node
- type: x-php-library
  url: https://github.com/contextio/PHP-ContextIO
- type: x-pricing
  url: http://context.io/pricing
- type: x-privacy
  url: http://www.returnpath.com/privacy-policy-data
- type: x-python-library
  url: https://github.com/contextio/Python-ContextIO
- type: x-ruby-library
  url: https://github.com/contextio/contextio-ruby
- type: x-selfservice-registration
  url: http://context.io/#signup
- type: x-terms-of-service
  url: http://context.io/terms-of-service
- type: x-twitter
  url: https://twitter.com/contextio
- type: x-website
  url: http://context.io/
- type: x-website
  url: http://context.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---