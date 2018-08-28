---
swagger: "2.0"
x-collection-name: Automox
x-complete: 0
info:
  title: Automox Get Servergroups
  description: Gets all `Server Group` objects for authenticated user
  termsOfService: https://www.automox.com/
  contact:
    name: support@automox.com
  version: 1.0.0
host: console.automox.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /servers:
    get:
      summary: Get Servers
      description: Gets all `Server` objects for authenticated user
      operationId: gets-all-server-objects-for-authenticated-user
      x-api-path-slug: servers-get
      parameters:
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servers
  /servers/{id}:
    get:
      summary: Get Servers
      description: Gets a specific `Server` object for the authenticated user.
      operationId: gets-a-specific-server-object-for-the-authenticated-user
      x-api-path-slug: serversid-get
      parameters:
      - in: path
        name: id
        description: Server (endpoint) ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servers
    put:
      summary: Put Servers
      description: Updates a `Server` object
      operationId: updates-a-server-object
      x-api-path-slug: serversid-put
      parameters:
      - in: path
        name: id
        description: Server (endpoint) ID
      - in: query
        name: o
        description: Organization ID
      - in: body
        name: server
        description: Updated server object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Servers
    delete:
      summary: Delete Servers
      description: ""
      operationId: ""
      x-api-path-slug: serversid-delete
      parameters:
      - in: path
        name: id
        description: Server (endpoint) ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servers
  /servers/{id}/packages:
    get:
      summary: Get Servers Packages
      description: Returns the command queue for the specified server (endpoint)
      operationId: returns-the-command-queue-for-the-specified-server-endpoint
      x-api-path-slug: serversidpackages-get
      parameters:
      - in: path
        name: id
        description: Server (endpoint) ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servers
      - Packages
  /servers/{id}/queues:
    get:
      summary: Get Servers Queues
      description: Returns the command queue for the specified server (endpoint)
      operationId: returns-the-command-queue-for-the-specified-server-endpoint
      x-api-path-slug: serversidqueues-get
      parameters:
      - in: path
        name: id
        description: Server (endpoint) ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servers
      - Queues
    post:
      summary: Post Servers Queues
      description: Issue a command to an endpoint. Can be used to install a specific
        set of patches or reboot an endpoint
      operationId: issue-a-command-to-an-endpoint-can-be-used-to-install-a-specific-set-of-patches-or-reboot-an-endpoin
      x-api-path-slug: serversidqueues-post
      parameters:
      - in: body
        name: command
        description: Command object
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Server (endpoint) ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servers
      - Queues
  /servergroups:
    get:
      summary: Get Servergroups
      description: Gets all `Server Group` objects for authenticated user
      operationId: gets-all-server-group-objects-for-authenticated-user
      x-api-path-slug: servergroups-get
      parameters:
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servergroups
    post:
      summary: Post Servergroups
      description: Updates a `Server Group` object
      operationId: updates-a-server-group-object
      x-api-path-slug: servergroups-post
      parameters:
      - in: body
        name: servergroup
        description: Updated server object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Servergroups
  /servergroups/{id}:
    get:
      summary: Get Servergroups
      description: Gets a specific `Server Group` object for the authenticated user.
      operationId: gets-a-specific-server-group-object-for-the-authenticated-user
      x-api-path-slug: servergroupsid-get
      parameters:
      - in: path
        name: id
        description: Server Group ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servergroups
    put:
      summary: Put Servergroups
      description: Updates a `Server Group` object
      operationId: updates-a-server-group-object
      x-api-path-slug: servergroupsid-put
      parameters:
      - in: path
        name: id
        description: Server Group ID
      - in: query
        name: o
        description: Organization ID
      - in: body
        name: servergroup
        description: Updated server object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Servergroups
    delete:
      summary: Delete Servergroups
      description: ""
      operationId: ""
      x-api-path-slug: servergroupsid-delete
      parameters:
      - in: path
        name: id
        description: Server Group ID
      - in: query
        name: o
        description: Organization ID
      responses:
        200:
          description: OK
      tags:
      - Servergroups
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