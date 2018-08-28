---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Post Projects Merge Requests Merge Request Todo
  version: 1.0.0
  description: Post projects merge requests merge request todo.
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/merge_requests/{merge_request_id}/todo:
    post:
      summary: Post Projects Merge Requests Merge Request Todo
      description: Post projects merge requests merge request todo.
      operationId: postV3ProjectsIdMergeRequestsMergeRequestIdTodo
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idtodo-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
        description: The ID of an issuable
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Todo
  /v3/projects/{id}/issues/{issue_id}/todo:
    post:
      summary: Post Projects Issues Issue Todo
      description: Post projects issues issue todo.
      operationId: postV3ProjectsIdIssuesIssueIdTodo
      x-api-path-slug: v3projectsidissuesissue-idtodo-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: issue_id
        description: The ID of an issuable
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Issues
      - Issue
      - Todo
  /v3/projects/{id}/triggers/{token}:
    get:
      summary: Get Projects Triggers Token
      description: Get specific trigger of a project
      operationId: getV3ProjectsIdTriggersToken
      x-api-path-slug: v3projectsidtriggerstoken-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: token
        description: The unique token of trigger
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Triggers
      - Token
    delete:
      summary: Delete Projects Triggers Token
      description: Delete projects triggers token.
      operationId: deleteV3ProjectsIdTriggersToken
      x-api-path-slug: v3projectsidtriggerstoken-delete
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: token
        description: The unique token of trigger
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Triggers
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