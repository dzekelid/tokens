---
swagger: "2.0"
x-collection-name: Apigee
x-complete: 0
info:
  title: Apigee Edge Post Organizations Name Oauth2 Accesstokens Access Token
  description: Revokes a specific access token.
  version: 1.0.0
host: api.enterprise.apigee.com
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/{org_name}/oauth1/accesstokens/{access_token}:
    get:
      summary: Get Organizations Name Oauth1 Accesstokens Access Token
      description: Fetches the details of given access token.
      operationId: getOrganizationsOrgNameOauth1AccesstokensAccessToken
      x-api-path-slug: organizationsorg-nameoauth1accesstokensaccess-token-get
      parameters:
      - in: path
        name: access_token
        description: Mention the access token
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth1
      - Accesstokens
      - Access
      - Token
    post:
      summary: Post Organizations Name Oauth1 Accesstokens Access Token
      description: Revokes the specified access token.
      operationId: postOrganizationsOrgNameOauth1AccesstokensAccessToken
      x-api-path-slug: organizationsorg-nameoauth1accesstokensaccess-token-post
      parameters:
      - in: path
        name: access_token
        description: Mention the access token
      - in: query
        name: action
        description: Mention action as revoke
      - in: query
        name: Content-Type
        description: Specify Content Type
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth1
      - Accesstokens
      - Access
      - Token
    delete:
      summary: Delete Organizations Name Oauth1 Accesstokens Access Token
      description: Deletes the specified access token.
      operationId: deleteOrganizationsOrgNameOauth1AccesstokensAccessToken
      x-api-path-slug: organizationsorg-nameoauth1accesstokensaccess-token-delete
      parameters:
      - in: path
        name: access_token
        description: Mention the access token
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth1
      - Accesstokens
      - Access
      - Token
  /organizations/{org_name}/oauth1/accesstokens:
    get:
      summary: Get Organizations Name Oauth1 Accesstokens
      description: Returns a count of all 1.0a access tokens in an orgnization .
      operationId: getOrganizationsOrgNameOauth1Accesstokens
      x-api-path-slug: organizationsorg-nameoauth1accesstokens-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth1
      - Accesstokens
  /organizations/{org_name}/oauth2/accesstokens/{access_token}:
    get:
      summary: Get Organizations Name Oauth2 Accesstokens Access Token
      description: Gets details of a specific access token.
      operationId: getOrganizationsOrgNameOauth2AccesstokensAccessToken
      x-api-path-slug: organizationsorg-nameoauth2accesstokensaccess-token-get
      parameters:
      - in: path
        name: access_token
        description: Mention the Access Token
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth2
      - Accesstokens
      - Access
      - Token
    post:
      summary: Post Organizations Name Oauth2 Accesstokens Access Token
      description: Revokes a specific access token.
      operationId: postOrganizationsOrgNameOauth2AccesstokensAccessToken
      x-api-path-slug: organizationsorg-nameoauth2accesstokensaccess-token-post
      parameters:
      - in: path
        name: access_token
        description: Mention the Access Token
      - in: query
        name: action
        description: Mention action as revoke
      - in: query
        name: Content-Type
        description: Specify Content Type
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth2
      - Accesstokens
      - Access
      - Token
    delete:
      summary: Delete Organizations Name Oauth2 Accesstokens Access Token
      description: Deletes a specific access token.
      operationId: deleteOrganizationsOrgNameOauth2AccesstokensAccessToken
      x-api-path-slug: organizationsorg-nameoauth2accesstokensaccess-token-delete
      parameters:
      - in: path
        name: access_token
        description: Mention the Access Token
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth2
      - Accesstokens
      - Access
      - Token
  /organizations/{org_name}/oauth2/accesstokens:
    get:
      summary: Get Organizations Name Oauth2 Accesstokens
      description: Get count of OAuth 2.0 access tokens under an organization .
      operationId: getOrganizationsOrgNameOauth2Accesstokens
      x-api-path-slug: organizationsorg-nameoauth2accesstokens-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth2
      - Accesstokens
  /organizations/{org_name}/oauth1/requesttokens/{request_token}:
    get:
      summary: Get Organizations Name Oauth1 Requesttokens Request Token
      description: Gets the Oauth 1.0 a request token for the speficied consumer key.
      operationId: getOrganizationsOrgNameOauth1RequesttokensRequestToken
      x-api-path-slug: organizationsorg-nameoauth1requesttokensrequest-token-get
      parameters:
      - in: query
        name: consumerKey
        description: Mention valid consumer key
      - in: query
        name: Content-Type
        description: Specify Content Type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: request_token
        description: Mention the request token
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth1
      - Requesttokens
      - Request
      - Token
    post:
      summary: Post Organizations Name Oauth1 Requesttokens Request Token
      description: Revokes an OAuth 1.0 a request token.
      operationId: postOrganizationsOrgNameOauth1RequesttokensRequestToken
      x-api-path-slug: organizationsorg-nameoauth1requesttokensrequest-token-post
      parameters:
      - in: query
        name: action
        description: Mention action as revoke
      - in: query
        name: Content-Type
        description: Specify Content Type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: request_token
        description: Mention the request token
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth1
      - Requesttokens
      - Request
      - Token
    delete:
      summary: Delete Organizations Name Oauth1 Requesttokens Request Token
      description: Deletes the request token specified.
      operationId: deleteOrganizationsOrgNameOauth1RequesttokensRequestToken
      x-api-path-slug: organizationsorg-nameoauth1requesttokensrequest-token-delete
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: request_token
        description: Mention the request token
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth1
      - Requesttokens
      - Request
      - Token
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---