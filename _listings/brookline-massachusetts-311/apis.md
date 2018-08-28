---
name: Brookline Massachusetts 311
x-slug: brookline-massachusetts-311
description: The 311 website for Brookline Massachusetts.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
  Shot 2017-12-26 at 9.54.50 PM.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Tokens
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/brookline-massachusetts-311/apis.md
specificationVersion: "0.14"
apis:
- name: Brookline MA Open311 GeoReport API - Id Of Service_request Via Token
  x-api-slug: tokenstoken-id-response-format-get
  description: Get the service_request_id from a temporary token. This is unnecessary
    if the response from creating a service request does not contain a token.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-12-26 at 9.54.50 PM.png
  humanURL: http://spot.brooklinema.gov/open311
  baseURL: https://spot.brooklinema.gov//open311/v2/
  tags: 311, Open311
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/brookline-massachusetts-311/tokenstoken-id-response-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/brookline-massachusetts-311/tokenstoken-id-response-format-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://baltimore.open311.api.gallery.streamdata.io
- type: x-open-311-feed
  url: http://spot.brooklinema.gov/open311/v2/services.xml?jurisdiction_id=brooklinema.gov
- type: x-website
  url: http://spot.brooklinema.gov/open311
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---