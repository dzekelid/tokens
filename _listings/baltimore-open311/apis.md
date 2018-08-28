---
name: Baltimore Open311
x-slug: baltimore-open311
description: Baltimore 311 helps residents make their neighborhoods more beautiful
  by reporting local issues including potholes, graffiti, and streetlight outages.
  Residents can track the status of reports they or other members of the community
  have submitted
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/baltimore311-logo.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Tokens
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/baltimore-open311/apis.md
specificationVersion: "0.14"
apis:
- name: Open311 GeoReport API - Id Of Service_request Via Token
  x-api-slug: tokenstoken-id-response-format-get
  description: Get the service_request_id from a temporary token. This is unnecessary
    if the response from creating a service request does not contain a token.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/baltimore311-logo.png
  humanURL: http://wiki.open311.org/GeoReport_v2/Servers
  baseURL: https://311.baltimorecity.gov//open311/v2/
  tags: Government, Open311, 311, API Provider, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/baltimore-open311/tokenstoken-id-response-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/baltimore-open311/tokenstoken-id-response-format-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.waf.api.gallery.streamdata.io
- type: x-website
  url: http://wiki.open311.org/GeoReport_v2/Servers
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---