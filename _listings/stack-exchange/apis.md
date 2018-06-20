---
name: Stack Exchange
x-slug: stack-exchange
description: After someone asks a question, members of the community propose answers.
  Others vote on those answers. Very quickly, the answers with the most votes rise
  to the top. You don???t have to read through a lot of discussion to find the best
  answer.    Like to...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
x-kinRank: "8"
x-alexaRank: "126"
tags: Tokens
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/stack-exchange/apis.md
specificationVersion: "0.14"
apis:
- name: Stack Exchange Get Acces Tokens
  x-api-slug: stack-exchange
  description: "Reads the properties for a set of access tokens.\n \n{accessTokens}
    can contain up to 20 access tokens. These are obtained by authenticating a user
    using OAuth 2.0.\n \nThis method returns a list of access_tokens."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//access-tokens/{accessTokens}
  tags: Authentication,Access Tokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/stack-exchange/accesstokensaccesstokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/stack-exchange/accesstokensaccesstokens-get-openapi.md
- name: Stack Exchange Invalidate Acces Tokens
  x-api-slug: stack-exchange
  description: "Immediately expires the access tokens passed. This method is meant
    to allow an application to discard any active access tokens it no longer needs.\n
    \n{accessTokens} can contain up to 20 access tokens. These are obtained by authenticating
    a user using OAuth 2.0.\n \nThis method returns a list of access_tokens."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//access-tokens/{accessTokens}/invalidate
  tags: Authentication,Access Tokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/stack-exchange/accesstokensaccesstokensinvalidate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/stack-exchange/accesstokensaccesstokensinvalidate-get-openapi.md
- name: Stack Exchange De-Authenticate Token
  x-api-slug: stack-exchange
  description: "Passing valid access_tokens to this method causes the application
    that created them to be de-authorized by the user associated with each access_token.
    This will remove the application from their apps tab, and cause all other existing
    access_tokens to be destroyed.\n \nThis method is meant for uninstalling applications,
    recovering from access_token leaks, or simply as a stronger form of /access-tokens/{accessTokens}/invalidate.\n
    \nNothing prevents a user from re-authenticate to an application that has de-authenticated
    itself, the user will be prompted to approve the application again however.\n
    \n{accessTokens} can contain up to 20 access tokens. These are obtained by authenticating
    a user using OAuth 2.0.\n \nThis method returns a list of access_tokens."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2//apps/{accessTokens}/de-authenticate
  tags: Authentication,Access Tokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/stack-exchange/appsaccesstokensdeauthenticate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/stack-exchange/appsaccesstokensdeauthenticate-get-openapi.md
- name: Stack Exchange
  x-api-slug: stack-exchange
  description: After someone asks a question, members of the community propose answers.
    Others vote on those answers. Very quickly, the answers with the most votes rise
    to the top. You don???t have to read through a lot of discussion to find the best
    answer.    Like to...
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/253-stack-exchange.jpg
  humanURL: http://stackexchange.com
  baseURL: https://api.stackexchange.com//2.2
  tags: Tokens
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/stack-exchange/openapi.md
x-common:
- type: x-authentication
  url: https://api.stackexchange.com/docs/authentication
- type: x-base
  url: https://api.stackexchange.com/
- type: x-blog
  url: http://stackexchange.com/blogs
- type: x-blog-rss
  url: http://blog.stackoverflow.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stack-exchange
- type: x-crunchbase
  url: https://crunchbase.com/organization/stack-exchange
- type: x-developer
  url: http://api.stackexchange.com/
- type: x-email
  url: legal@stackexchange.com
- type: x-email
  url: team@stackexchange.com
- type: x-email
  url: team+api@stackexchange.com
- type: x-error-codes
  url: https://api.stackexchange.com/docs/error-handling
- type: x-github
  url: https://github.com/StackExchange
- type: x-javascript-sdk
  url: https://api.stackexchange.com/docs/js-lib
- type: x-privacy
  url: https://stackexchange.com/legal/privacy-policy
- type: x-rate-limits
  url: https://api.stackexchange.com/docs/throttle
- type: x-selfservice-registration
  url: https://stackapps.com/users/login?returnurl=/apps/oauth/register
- type: x-support
  url: https://stackexchange.com/about/contact
- type: x-terms-of-service
  url: http://stackexchange.com/legal/api-terms-of-use
- type: x-twitter
  url: https://twitter.com/StackExchange
- type: x-website
  url: http://stackexchange.com
- type: x-website
  url: https://stackexchange.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---