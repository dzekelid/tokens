---
name: Authentiq Connect
x-slug: authentiq-connect
description: Authentiq offers the convenience of passwordless authentication with
  the safety of two step verification. Sign up for Authentiq today, and never think
  about authentication again.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/authentiq-logo.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Tokens
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/authentiq-connect/apis.md
specificationVersion: "0.14"
apis:
- name: Authentiq Connect - Obtain an ID Token
  x-api-slug: token-post
  description: |-
    Exchange en authorization code for an ID Token or Access Token.

    This endpoint supports both `client_secret_post` and `client_secret_basic` authenticatino methods, as specified by the client's `token_endpoint_auth_method`.

    See also:
      - [OIDC Token Endpoint](http://openid.net/specs/openid-connect-core-1_0.html#TokenRequest)
      - [OIDC Successful Token response](http://openid.net/specs/openid-connect-core-1_0.html#TokenResponse)
      - [OIDC Token Error response](http://openid.net/specs/openid-connect-core-1_0.html#TokenError)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/authentiq-logo.png
  humanURL: http://authentiq.com
  baseURL: https://connect.authentiq.io//
  tags: Authentication, Passwords, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/authentiq-connect/token-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/authentiq-connect/token-post-openapi.md
- name: Authentiq Connect - Obtain an ID Token
  x-api-slug: token-post
  description: |-
    Exchange en authorization code for an ID Token or Access Token.

    This endpoint supports both `client_secret_post` and `client_secret_basic` authenticatino methods, as specified by the client's `token_endpoint_auth_method`.

    See also:
      - [OIDC Token Endpoint](http://openid.net/specs/openid-connect-core-1_0.html#TokenRequest)
      - [OIDC Successful Token response](http://openid.net/specs/openid-connect-core-1_0.html#TokenResponse)
      - [OIDC Token Error response](http://openid.net/specs/openid-connect-core-1_0.html#TokenError)
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/authentiq-logo.png
  humanURL: http://authentiq.com
  baseURL: https://connect.authentiq.io//
  tags: Authentication, Passwords, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/authentiq-connect/token-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/authentiq-connect/token-post-openapi.md
x-common:
- type: x-website
  url: http://authentiq.com
- type: x-api-gallery
  url: http://auth0.api.gallery.streamdata.io
- type: x-api-stack
  url: http://authentiq.connect.stack.network
- type: x-blog
  url: https://www.authentiq.com/blog/
- type: x-developer
  url: https://www.authentiq.com/developers/
- type: x-github
  url: https://github.com/AuthentiqID
- type: x-pricing
  url: https://www.authentiq.com/pricing/
- type: x-twitter
  url: AuthentiqID
- type: x-website
  url: http://authentiq.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---