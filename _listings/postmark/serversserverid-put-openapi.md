---
swagger: "2.0"
x-collection-name: Postmark
x-complete: 0
info:
  title: Postmark Account Edit a Server
  description: Edit a server.
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
  /server:
    parameters:
      summary: Parameters Server
      description: Parameters server.
      operationId: parametersServer
      x-api-path-slug: server-parameters
      responses:
        200:
          description: OK
      tags:
      - Server
    get:
      summary: Get Server
      description: Gets the server details and figures out your unique InboundHash
        where you can forward your email. This can be found in the web app in your
        server's Credentials tab or via the API.
      operationId: getServer
      x-api-path-slug: server-get
      parameters:
      - in: query
        name: Accept
        description: The accepted type for the response
      - in: query
        name: Content-Type
        description: The content type of the request
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Server
    post:
      summary: Post Server
      description: Sets the URL where we should send JSON data. In order for your
        application receive the emails that we parse, you will need to tell Postmark
        where to send the JSON data for each inbound email it processes, which is
        done via an HTTP POST to a URL of your choice. You can set this URL in the
        Settings page for your Postmark server in the web app, or using the InboundHookUrl
        field in the API. It also lets you choose a domain that you would like to
        listen on for incoming email to be processed by Postmark. We recommend a separate
        subdomain, like inbound.yourdomain.com. Each server can listen to one unique
        domain, so make sure to set the X-Postmark-Server-Token to the correct server
        token in the API call below.
      operationId: postServer
      x-api-path-slug: server-post
      parameters:
      - in: query
        name: Accept
        description: The accepted type for the response
      - in: query
        name: Content-Type
        description: The content type of the request
      responses:
        200:
          description: OK
      tags:
      - Server
    put:
      summary: Put Server
      description: Put server.
      operationId: putServer
      x-api-path-slug: server-put
      parameters:
      - in: body
        name: body
        description: The settings that should be modified for the current server
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Server
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