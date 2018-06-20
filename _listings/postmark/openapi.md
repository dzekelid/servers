---
swagger: "2.0"
x-collection-name: Postmark
x-complete: 1
info:
  title: Postmark Account-level
  description: postmark-makes-sending-and-receiving-email-incredibly-easy--the-accountlevel-api-allows-users-toconfigure-all-servers-domains-and-sender-signatures-associated-with-an-account-
  version: 0.9.0
host: api.postmarkapp.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /servers:
    get:
      summary: List servers
      description: List servers.
      operationId: listServers
      x-api-path-slug: servers-get
      parameters:
      - in: query
        name: count
        description: Number of servers to return per request
      - in: query
        name: name
        description: Filter by a specific server name
      - in: query
        name: offset
        description: Number of servers to skip
      - in: header
        name: X-Postmark-Account-Token
        description: The token associated with the Account on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Servers
    post:
      summary: Create a Server
      description: Create a server.
      operationId: createServer
      x-api-path-slug: servers-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Postmark-Account-Token
        description: The token associated with the Account on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Servers
  /servers/{serverid}:
    delete:
      summary: Delete a Server
      description: Delete a server.
      operationId: deleteServer
      x-api-path-slug: serversserverid-delete
      parameters:
      - in: path
        name: serverid
        description: The ID of the Server that should be deleted
      - in: header
        name: X-Postmark-Account-Token
        description: The token associated with the Account on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Servers
      - Serverid
    get:
      summary: Get a Server
      description: Get a server.
      operationId: getServerInformation
      x-api-path-slug: serversserverid-get
      parameters:
      - in: path
        name: serverid
        description: The ID of the Server to get
      - in: header
        name: X-Postmark-Account-Token
        description: The token associated with the Account on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Servers
      - Serverid
    put:
      summary: Edit a Server
      description: Edit a server.
      operationId: editServerInformation
      x-api-path-slug: serversserverid-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: serverid
        description: The ID of the Server to update
      - in: header
        name: X-Postmark-Account-Token
        description: The token associated with the Account on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Servers
      - Serverid
---