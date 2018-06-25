---
name: Server Density
x-slug: server-density
description: SaaS infrastructure monitoring. Dashboards, graphs and alerts to help
  you improve performance and maintain uptime. Organizer of @humanops
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
x-kinRank: "7"
x-alexaRank: "209719"
tags: Tokens
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/server-density/apis.md
specificationVersion: "0.14"
apis:
- name: Tokens API Getting a token via the API
  x-api-slug: tokens-api
  description: |-
    If you need to generate tokens programmatically, you can request a token through the API with your username and password. All future requests can then be performed using the returned token.
    If the user generating the token has Multi Factor Authentication enabled, you cannot use this method and must create the token via the web UI.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///tokens
  tags: Tokens
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/server-density/tokens--openapi.md
- name: Tokens API Create a token
  x-api-slug: tokens-api
  description: Create a token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///tokens/
  tags: Tokens
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/server-density/tokens--openapi.md
- name: Tokens API Delete a token
  x-api-slug: tokens-api
  description: Delete a token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io.///tokens/tokenId
  tags: Tokens
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/server-density/tokenstokenid--openapi.md
- name: Tokens API
  x-api-slug: tokens-api
  description: SaaS infrastructure monitoring. Dashboards, graphs and alerts to help
    you improve performance and maintain uptime. Organizer of @humanops
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/475-server-density.jpg
  humanURL: https://www.serverdensity.com
  baseURL: ://api.serverdensity.io./
  tags: Tokens
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/server-density/openapi.md
x-common:
- type: x-website
  url: https://www.serverdensity.com
- type: x-blog
  url: http://blog.serverdensity.com/
- type: x-blog-rss
  url: http://feeds.feedburner.com/serverdensity
- type: x-crunchbase
  url: https://crunchbase.com/organization/server-density
- type: x-crunchbase
  url: http://www.crunchbase.com/company/server-density
- type: x-email
  url: hello@serverdensity.com
- type: x-github
  url: https://github.com/serverdensity
- type: x-linkedin
  url: https://www.linkedin.com/company/server-density
- type: x-twitter
  url: https://twitter.com/serverdensity
- type: x-website
  url: http://www.serverdensity.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---