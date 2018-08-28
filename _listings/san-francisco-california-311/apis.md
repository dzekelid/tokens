---
name: San Francisco California 311
x-slug: san-francisco-california-311
description: The 311 service for the City of San Francisco, California.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/vzN3Pt2u_400x400.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Tokens
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/san-francisco-california-311/apis.md
specificationVersion: "0.14"
apis:
- name: San Francisco CA Open311 GeoReport API - Id Of Service_request Via Token
  x-api-slug: tokenstoken-id-response-format-get
  description: Get the service_request_id from a temporary token. This is unnecessary
    if the response from creating a service request does not contain a token.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/vzN3Pt2u_400x400.png
  humanURL: http://ouc.dc.gov
  baseURL: https://mobile311.sfgov.org//open311/v2/
  tags: 311, Open311
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/san-francisco-california-311/tokenstoken-id-response-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/san-francisco-california-311/tokenstoken-id-response-format-get-openapi.md
x-common:
- type: x-twitter
  url: https://twitter.com/311DCgov
- type: x-website
  url: http://ouc.dc.gov
- type: x-api-gallery
  url: http://rat.genome.database.api.gallery.streamdata.io
- type: x-open-311-feed
  url: http://mobile311.sfgov.org/open311/v2/services.xml?jurisdiction_id=sfgov.org
- type: x-website
  url: https://sf311.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---