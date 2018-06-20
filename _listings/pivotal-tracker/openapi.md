---
swagger: "2.0"
x-collection-name: Pivotal Tracker
x-complete: 1
info:
  title: Pivotal Tracker
  description: access-and-manipulate-agile-project-management-data-including-projects-stories-and-tasks-
  version: 1.0.0
host: www.pivotaltracker.com
basePath: /services/v3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tokens/active:
    get:
      summary: Get Tokens Active
      description: Returns an API token associated with the user. This method requires
        HTTP Basic authentication.
      operationId: getTokensActive
      x-api-path-slug: tokensactive-get
      responses:
        200:
          description: OK
      tags:
      - Tokens
      - Active
    post:
      summary: Post Tokens Active
      description: Returns an API token associated with the user.
      operationId: postTokensActive
      x-api-path-slug: tokensactive-post
      parameters:
      - in: query
        name: password
        description: The users password
      - in: query
        name: username
        description: The users name
      responses:
        200:
          description: OK
      tags:
      - Tokens
      - Active
---