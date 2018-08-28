---
name: Urban Airship
x-slug: urban-airship
description: A market-leading mobile app engagement, mobile analytics, mobile data
  integration and mobile wallet marketing solution.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
x-kinRank: "8"
x-alexaRank: "79571"
tags: Tokens
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/apis.md
specificationVersion: "0.14"
apis:
- name: Urban Airship - Put Device Tokens Token
  x-api-slug: device-tokenstoken-put
  description: Registers a device token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenstoken-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenstoken-put-openapi.md
- name: Urban Airship - Get Device Tokens Token
  x-api-slug: device-tokenstoken-get
  description: Gets a device token???s alias.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenstoken-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenstoken-get-openapi.md
- name: Urban Airship - Delete Device Tokens Token
  x-api-slug: device-tokenstoken-delete
  description: Marks the device token as inactive. No notifications will be delivered
    to it until a PUT is executed again. The DELETE returns HTTP 204 No Content, and
    needs no payload. When a token is deleted in this manner, any alias or tags will
    be cleared.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenstoken-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenstoken-delete-openapi.md
- name: Urban Airship - Get Device Tokens
  x-api-slug: device-tokens-get
  description: Gets information about all of your device tokens. If your application
    has a large number of device tokens, we???ll paginate the request for you. By
    default, we paginate at 5000 device tokens. You can receive the next page simply
    by retrieving the URL from "next_page" - in this way it is easy to export all
    of your device tokens and all their data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokens-get-openapi.md
- name: Urban Airship - Get Device Tokens Count
  x-api-slug: device-tokenscount-get
  description: Gets the number of device tokens you have registered.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenscount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenscount-get-openapi.md
- name: Urban Airship - Get Device Tokens Feedback
  x-api-slug: device-tokensfeedback-get
  description: Gets what device tokens are now invalid. Apple informs us when a push
    notification is sent to a device that can???t receive it because the application
    has been uninstalled. We mark the device token as inactive and immediately stop
    sending notifications to that device. Once a day is a good interval for querying
    the feedback service, but you can do it more often to save on bandwidth from unnecessary
    notifications. In the response, what does marked_inactive_on mean? Apple sends
    a timestamp for each device token returned via the feedback service. Since a device
    can be off the network for a while, this can be a point in the recent past. In
    order to make this API work smoothly for you, we record the timestamp we marked
    as inactive. This means you only need to query for data since the last time you
    queried. Once a day is a good timeframe, or once a week for very small or infrequently
    used applications. A few times a day is good for applications with heavy use.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensfeedback-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensfeedback-get-openapi.md
- name: Urban Airship - Get Device Tokens Device Token Tags
  x-api-slug: device-tokensdevice-tokentags-get
  description: Gets tags for a specific device token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensdevice-tokentags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensdevice-tokentags-get-openapi.md
- name: Urban Airship - Put Device Tokens Device Token Tags Tag
  x-api-slug: device-tokensdevice-tokentagstag-put
  description: Creates a tag and associate it with the specific device token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensdevice-tokentagstag-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensdevice-tokentagstag-put-openapi.md
- name: Urban Airship - Delete Device Tokens Device Token Tags Tag
  x-api-slug: device-tokensdevice-tokentagstag-delete
  description: Removes a single tag from a device token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensdevice-tokentagstag-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensdevice-tokentagstag-delete-openapi.md
- name: Urban Airship - Put Device Tokens Token
  x-api-slug: device-tokenstoken-put
  description: Registers a device token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenstoken-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenstoken-put-openapi.md
- name: Urban Airship - Get Device Tokens Token
  x-api-slug: device-tokenstoken-get
  description: Gets a device token???s alias.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenstoken-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenstoken-get-openapi.md
- name: Urban Airship - Delete Device Tokens Token
  x-api-slug: device-tokenstoken-delete
  description: Marks the device token as inactive. No notifications will be delivered
    to it until a PUT is executed again. The DELETE returns HTTP 204 No Content, and
    needs no payload. When a token is deleted in this manner, any alias or tags will
    be cleared.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenstoken-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenstoken-delete-openapi.md
- name: Urban Airship - Get Device Tokens Device Token Tags
  x-api-slug: device-tokensdevice-tokentags-get
  description: Gets tags for a specific device token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensdevice-tokentags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensdevice-tokentags-get-openapi.md
- name: Urban Airship - Put Device Tokens Device Token Tags Tag
  x-api-slug: device-tokensdevice-tokentagstag-put
  description: Creates a tag and associate it with the specific device token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensdevice-tokentagstag-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensdevice-tokentagstag-put-openapi.md
- name: Urban Airship - Delete Device Tokens Device Token Tags Tag
  x-api-slug: device-tokensdevice-tokentagstag-delete
  description: Removes a single tag from a device token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensdevice-tokentagstag-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensdevice-tokentagstag-delete-openapi.md
- name: Urban Airship - Delete Device Tokens Device Token Tags Tag
  x-api-slug: device-tokensdevice-tokentagstag-delete
  description: Removes a single tag from a device token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensdevice-tokentagstag-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensdevice-tokentagstag-delete-openapi.md
- name: Urban Airship - Put Device Tokens Device Token Tags Tag
  x-api-slug: device-tokensdevice-tokentagstag-put
  description: Creates a tag and associate it with the specific device token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensdevice-tokentagstag-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensdevice-tokentagstag-put-openapi.md
- name: Urban Airship - Get Device Tokens Device Token Tags
  x-api-slug: device-tokensdevice-tokentags-get
  description: Gets tags for a specific device token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensdevice-tokentags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokensdevice-tokentags-get-openapi.md
- name: Urban Airship - Delete Device Tokens Token
  x-api-slug: device-tokenstoken-delete
  description: Marks the device token as inactive. No notifications will be delivered
    to it until a PUT is executed again. The DELETE returns HTTP 204 No Content, and
    needs no payload. When a token is deleted in this manner, any alias or tags will
    be cleared.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenstoken-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenstoken-delete-openapi.md
- name: Urban Airship - Get Device Tokens Token
  x-api-slug: device-tokenstoken-get
  description: Gets a device token???s alias.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenstoken-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenstoken-get-openapi.md
- name: Urban Airship - Put Device Tokens Token
  x-api-slug: device-tokenstoken-put
  description: Registers a device token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenstoken-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tokens/master/_listings/urban-airship/device-tokenstoken-put-openapi.md
x-common:
- type: x-website
  url: http://urbanairship.com/
- type: x-android-sdk
  url: http://docs.urbanairship.com/platform/android.html
- type: x-api-gallery
  url: http://ulster.bank.api.gallery.streamdata.io
- type: x-api-stack
  url: http://urban.airship.stack.network
- type: x-blackberry-sdk
  url: http://docs.urbanairship.com/platform/blackberry.html
- type: x-blog
  url: http://urbanairship.com/blog
- type: x-blog-rss
  url: http://urbanairship.com/blog/rss
- type: x-case-studies
  url: http://urbanairship.com/resources/case-studies
- type: x-crunchbase
  url: http://www.crunchbase.com/company/urban-airship
- type: x-crunchbase
  url: https://crunchbase.com/organization/urban-airship
- type: x-developer
  url: http://docs.urbanairship.com/
- type: x-email
  url: legal@urbanairship.com
- type: x-email
  url: privacy@urbanairship.com
- type: x-email
  url: support@urbanairship.com
- type: x-github
  url: https://github.com/urbanairship
- type: x-glossary
  url: http://docs.urbanairship.com/reference/glossary.html
- type: x-ios-sdk
  url: http://docs.urbanairship.com/platform/ios.html
- type: x-linkedin
  url: https://www.linkedin.com/company/urban-airship/
- type: x-phonegap-sdk
  url: http://docs.urbanairship.com/platform/phonegap.html
- type: x-pricing
  url: https://www.urbanairship.com/products/engage/pricing
- type: x-privacy
  url: http://urbanairship.com/legal/privacy-policy
- type: x-security
  url: http://docs.urbanairship.com/reference/app_keys_secrets.html
- type: x-twitter
  url: https://twitter.com/urbanairship
- type: x-website
  url: http://urbanairship.com
- type: x-white-papers
  url: http://urbanairship.com/resources/whitepapers
- type: x-windows-sdk
  url: http://docs.urbanairship.com/platform/windows.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---