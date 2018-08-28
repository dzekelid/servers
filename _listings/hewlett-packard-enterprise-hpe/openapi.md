swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 1
info:
  title: HPE OneSphere API
  description: hpe-onesphere-hybrid-cloud-management-rest-api-for-calls-requiring-authentication-use-restsession-to-get-a-token-
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
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
      description: Returns servers.
      operationId: GetServer
      x-api-path-slug: servers-get
      parameters:
      - in: query
        name: applianceUri
        description: Set of servers in this appliance
      - in: query
        name: regionUri
        description: Set of servers in this region
      - in: query
        name: zoneUri
        description: Set of servers in this zone
      responses:
        200:
          description: OK
      tags:
      - Servers
    post:
      summary: Post Servers
      description: Create/Register a server.
      operationId: CreateServer
      x-api-path-slug: servers-post
      parameters:
      - in: body
        name: server
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Servers
  /servers/{id}:
    delete:
      summary: Delete Servers
      description: |-
        Delete a server.
        Note that by default only servers created via the HPE OneSphere API can be
        subsequently deleted. HPE OneSphere managed servers (those that have
        an applianceUri) cannot be deleted via this operation (a '403' will be returned),
        unless the 'force' parameter is supplied and set to 'true'.
      operationId: DeleteServer
      x-api-path-slug: serversid-delete
      parameters:
      - in: query
        name: force
        description: Delete Server even if Delete operation is not allowed on this
          server by default,e
      - in: path
        name: id
        description: ID of the server to delete
      responses:
        200:
          description: OK
      tags:
      - Servers
    get:
      summary: Get Servers
      description: Returns a server based on its ID.
      operationId: GetServerById
      x-api-path-slug: serversid-get
      parameters:
      - in: path
        name: id
        description: ID of the server to retrieve
      responses:
        200:
          description: OK
      tags:
      - Servers
    patch:
      summary: Patch Servers
      description: Update properties of a server.
      operationId: UpdateServer
      x-api-path-slug: serversid-patch
      parameters:
      - in: body
        name: body
        description: List of server updates
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of server to update
      responses:
        200:
          description: OK
      tags:
      - Servers