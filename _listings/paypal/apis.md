---
name: PayPal
x-slug: paypal
description: PayPal is the faster, safer way to send money, make an online payment,
  receive money or set up a merchant account.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
x-kinRank: "10"
x-alexaRank: "71"
tags: Tokens
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/paypal/apis.md
specificationVersion: "0.14"
apis:
- name: Paypal GetAccess Token
  x-api-slug: paypal
  description: Use the GetAccessToken API operation to obtain an access token for
    a set of permissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////Permissions/GetAccessToken
  tags: Payments,Access Tokens
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/paypal/permissionsgetaccesstoken-post-openapi.md
- name: Paypal
  x-api-slug: paypal
  description: PayPal is the faster, safer way to send money, make an online payment,
    receive money or set up a merchant account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com//
  tags: Tokens
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/paypal/openapi.md
x-common:
- type: x-base-url
  url: https://api.paypal.com
- type: x-crunchbase
  url: https://crunchbase.com/organization/paypal
- type: x-crunchbase
  url: http://www.crunchbase.com/company/paypal
- type: x-developer
  url: https://developer.paypal.com/
- type: x-faq
  url: https://developer.paypal.com/docs/faq/
- type: x-getting-started
  url: https://developer.paypal.com/docs/
- type: x-github
  url: https://github.com/paypal
- type: x-playground
  url: https://devtools-paypal.com/hateoas/index.html
- type: x-privacy
  url: https://www.paypal.com/us/cgi-bin/webscr?cmd=p/gen/ua/policy_privacy-outside
- type: x-release-notes
  url: https://developer.paypal.com/docs/release-notes/
- type: x-terms-of-service
  url: https://cms.paypal.com/us/cgi-bin/?cmd=_render-content&content_ID=ua/Legal_Hub_full
- type: x-twitter
  url: https://twitter.com/paypal
- type: x-website
  url: https://paypal.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---