---
swagger: "2.0"
x-collection-name: Apigee
x-complete: 1
info:
  title: Apigee Edge
  description: restful-management-api-to-create-configure-and-manage-api-proxies-and-api-products-create-and-manage-apps-and-app-developers-and-more-
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
  /organizations/{org_name}/developers/{developer_email}/apps/{app_name}/oauth1accesstokens:
    get:
      summary: Get Organizations Name Developers Developer Email Apps App Name Oauth1accesstokens
      description: Get count of OAuth 1.0 access tokens for a developer's app.
      operationId: getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameOauth1accesstokens
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-nameoauth1accesstokens-get
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: developer_email
        description: Mention the developer email
      - in: path
        name: org_name
        description: Mention the organization Name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Oauth1accesstokens
  /organizations/{org_name}/developers/{developer_email}/apps/{app_name}/oauth2accesstokens:
    get:
      summary: Get Organizations Name Developers Developer Email Apps App Name Oauth2accesstokens
      description: Get count of    OAuth 2.0 access tokens for a developer's app.
      operationId: getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameOauth2accesstokens
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-nameoauth2accesstokens-get
      parameters:
      - in: query
        name: appName
        description: Mention the app name
      - in: query
        name: developerEmail
        description: Mention the developer email
      - in: query
        name: organizationName
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Oauth2accesstokens
  /organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}/oauth1accesstokens:
    get:
      summary: Get Organizations Name Developers Developer Email Apps App Name Keys
        Consumer Key Oauth1accesstokens
      description: Get count of OAuth 1.0 access tokens for a developer's app key.
      operationId: getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKeyOauth1accesstokens
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyoauth1accesstokens-get
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: consumer_key
        description: Mention the consumer key
      - in: path
        name: developer_email
        description: Mention the developer email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
      - Oauth1accesstokens
  /organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}/oauth2accesstokens:
    get:
      summary: Get Organizations Name Developers Developer Email Apps App Name Keys
        Consumer Key Oauth2accesstokens
      description: Get count of OAuth 2.0 access tokens for a developer's app key.
      operationId: getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKeyOauth2accesstokens
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyoauth2accesstokens-get
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: consumer_key
        description: Mention the consumer key
      - in: path
        name: developer_email
        description: Mention the developer name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
      - Oauth2accesstokens
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
  /organizations/{org_name}/oauth1/requesttokens:
    get:
      summary: Get Organizations Name Oauth1 Requesttokens
      description: Returns list of all OAuth 1.0a request.
      operationId: getOrganizationsOrgNameOauth1Requesttokens
      x-api-path-slug: organizationsorg-nameoauth1requesttokens-get
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
      - Requesttokens
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
---