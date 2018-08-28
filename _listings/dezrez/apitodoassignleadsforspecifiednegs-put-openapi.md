---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Assign InboundLead Todos to all the specified Negs using round-robin
    assignement.
  version: 1.0.0
  description: Assign inboundlead todos to all the specified negs using round-robin
    assignement..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/todo/getall:
    get:
      summary: "Get the list of all ToDo's if no parameter is sent;\r\n<param name=\"filterToDo\">if
        provided will filter by ToDo type</param><param name=\"pageSize\"></param><param
        name=\"pageNumber\"></param>"
      description: "Get the list of all todo's if no parameter is sent;\r\n<param
        name=\"filtertodo\">if provided will filter by todo type</param><param name=\"pagesize\"></param><param
        name=\"pagenumber\"></param>."
      operationId: DefaultToDo_GetAllBypageSizeBypageNumberByfilterToDo.filterCategoryByfilterToDo.toDoTypeByfilterToDo
      x-api-path-slug: apitodogetall-get
      parameters:
      - in: query
        name: filterToDo.branchId
      - in: query
        name: filterToDo.filterCategory
      - in: query
        name: filterToDo.negotiatorIds
      - in: query
        name: filterToDo.toDoType
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - ToDos
      - If
      - "No"
      - Parameter
      - Is
      - "Sent;\r\n<param"
      - Name=filterToDo>if
      - Provided
      - Will
      - Filter
      - By
      - ToDo
      - Type<
      - Param><param
      - Name=pageSize><
      - Param><param
      - Name=pageNumber><
      - Param>
  /api/todo/activetasks:
    get:
      summary: Get the list of active tasks of a Todo
      description: Get the list of active tasks of a todo.
      operationId: DefaultToDo_ActiveTasksBytoDoIdByignoreDueDateBypageSizeBypageNumber
      x-api-path-slug: apitodoactivetasks-get
      parameters:
      - in: query
        name: ignoreDueDate
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: toDoId
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Active
      - Tasks
      - Of
      - Todo
  /api/todo/completedtasks:
    get:
      summary: Get the list of completed tasks of a Todo
      description: Get the list of completed tasks of a todo.
      operationId: DefaultToDo_CompletedTasksBytoDoId
      x-api-path-slug: apitodocompletedtasks-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: toDoId
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Completed
      - Tasks
      - Of
      - Todo
  /api/todo/teamtodos:
    get:
      summary: Get the list of completed tasks of a Todo
      description: Get the list of completed tasks of a todo.
      operationId: DefaultToDo_TeamTodosBybranchId
      x-api-path-slug: apitodoteamtodos-get
      parameters:
      - in: query
        name: branchId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Completed
      - Tasks
      - Of
      - Todo
  /api/todo/reassigntodo:
    put:
      summary: Reassign a todo to different negotiator(s)
      description: Reassign a todo to different negotiator(s).
      operationId: DefaultToDo_ReassignTodoByreassignTodoCommandData
      x-api-path-slug: apitodoreassigntodo-put
      parameters:
      - in: body
        name: reassignTodoCommandData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Reassign
      - Todo
      - To
      - Different
      - Negotiator(s)
  /api/todo/addtodonote:
    post:
      summary: Add note for a ToDo
      description: Add note for a todo.
      operationId: DefaultToDo_AddToDoNoteBytoDoIdBynote
      x-api-path-slug: apitodoaddtodonote-post
      parameters:
      - in: body
        name: note
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: toDoId
      responses:
        200:
          description: OK
      tags:
      - Notea
      - ToDo
  /api/DefaultToDo/{id}:
    get:
      summary: Get a ToDo by Id
      description: Get a todo by id.
      operationId: DefaultToDo_GetByid
      x-api-path-slug: apidefaulttodoid-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - ToDo
      - By
      - Id
  /api/todo/event/savetodo:
    post:
      summary: Save or Updates a Event ToDo and and its tasks
      description: Save or updates a event todo and and its tasks.
      operationId: EventToDo_SaveToDoBytoDoSave
      x-api-path-slug: apitodoeventsavetodo-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: toDoSave
        description: A wrapper for the todo save data and the various data contracts
          needed
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Save
      - S
      - Event
      - ToDo
      - And
      - Its
      - Tasks
  /api/todo/event/addtasks:
    put:
      summary: Add tasks to a Event ToDo
      description: Add tasks to a event todo.
      operationId: EventToDo_AddTasksByaddEventTasksCommandDataContract
      x-api-path-slug: apitodoeventaddtasks-put
      parameters:
      - in: body
        name: addEventTasksCommandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Tasks
      - To
      - Event
      - ToDo
  /api/todo/general/savetodo:
    post:
      summary: "Saves or Updates a General ToDo \r\nThis is currently used to save
        quick reminders"
      description: "Saves or updates a general todo \r\nthis is currently used to
        save quick reminders."
      operationId: GeneralToDo_SaveToDoBytoDoSave
      x-api-path-slug: apitodogeneralsavetodo-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: toDoSave
        description: A wrapper for the todo save data and the various data contracts
          needed
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Saves
      - S
      - General
      - ToDo
      - This
      - Is
      - Currently
      - Used
      - To
      - Save
      - Quick
      - Reminders
  /api/todo/group/savetodo:
    post:
      summary: Saves or Updates a Group ToDo and its tasks
      description: Saves or updates a group todo and its tasks.
      operationId: GroupToDo_SaveToDoBytoDoSave
      x-api-path-slug: apitodogroupsavetodo-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: toDoSave
        description: A wrapper for the todo save data and the various data contracts
          needed
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Saves
      - S
      - Group
      - ToDo
      - Its
      - Tasks
  /api/todo/group/addtasks:
    put:
      summary: Add task to a Group ToDo
      description: Add task to a group todo.
      operationId: GroupToDo_AddTasksByaddTasksCommandDataContract
      x-api-path-slug: apitodogroupaddtasks-put
      parameters:
      - in: body
        name: addTasksCommandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Task
      - To
      - Group
      - ToDo
  /api/todo/group/getupcomingtask:
    get:
      summary: Get the todo and latest task for a group
      description: Get the todo and latest task for a group.
      operationId: GroupToDo_GetUpComingTaskBygroupId
      x-api-path-slug: apitodogroupgetupcomingtask-get
      parameters:
      - in: query
        name: groupId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Todo
      - Latest
      - Taska
      - Group
  /api/list/todos/filters/{id}:
    delete:
      summary: Marks Todo List Filter as deleted
      description: Marks todo list filter as deleted.
      operationId: List_DeleteTodoListFilterByid
      x-api-path-slug: apilisttodosfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Todo
      - List
      - Filter
      - As
      - Deleted
  /api/todo/property/savetodo:
    post:
      summary: Save or Updates a Property ToDo and and its tasks
      description: Save or updates a property todo and and its tasks.
      operationId: PropertyToDo_SaveToDoBytoDoSave
      x-api-path-slug: apitodopropertysavetodo-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: toDoSave
        description: A wrapper for the todo save data and the various data contracts
          needed
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Save
      - S
      - Property
      - ToDo
      - And
      - Its
      - Tasks
  /api/todo/property/addtasks:
    put:
      summary: Add tasks to a Property ToDo
      description: Add tasks to a property todo.
      operationId: PropertyToDo_AddTasksByaddPropertyTasksCommandDataContract
      x-api-path-slug: apitodopropertyaddtasks-put
      parameters:
      - in: body
        name: addPropertyTasksCommandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Tasks
      - To
      - Property
      - ToDo
  /api/list/todotasks/filters/{id}:
    delete:
      summary: Marks Todos task List Filter as deleted
      description: Marks todos task list filter as deleted.
      operationId: List_DeleteTodoTaskListFilterByid
      x-api-path-slug: apilisttodotasksfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Todos
      - Task
      - List
      - Filter
      - As
      - Deleted
  /api/todo/assignleadsforspecifiednegs:
    put:
      summary: Assign InboundLead Todos to all the specified Negs using round-robin
        assignement.
      description: Assign inboundlead todos to all the specified negs using round-robin
        assignement..
      operationId: DefaultToDo_AssignLeadsForSpecifiedNegsByassignPropertyLeadsCommandDataContract
      x-api-path-slug: apitodoassignleadsforspecifiednegs-put
      parameters:
      - in: body
        name: assignPropertyLeadsCommandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Assign
      - InboundLead
      - Todos
      - To
      - ""
      - Specified
      - Negs
      - Using
      - Round-robin
      - Assignement
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