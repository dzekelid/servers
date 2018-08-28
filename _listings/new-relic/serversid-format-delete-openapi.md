---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Delete Servers  . Format
  version: 1.0.0
  description: |-
    This API endpoint deletes a server and all of its reported data.

    WARNING: Only servers that have stopped reporting can be deleted. This is an irreversible process which
    will delete all reported data for this server.
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /servers/{id}.{format}:
    get:
      summary: Get Servers  . Format
      description: |-
        This API endpoint returns a single Server, identified by ID. The time range for summary data is the last 10 minutes.???

        See our documentation for a discussion on
        summary data output.
      operationId: getServers.Format
      x-api-path-slug: serversid-format-get
      parameters:
      - in: path
        name: id
        description: Server ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Servers
      - ""
      - .
      - Format
    put:
      summary: Put Servers  . Format
      description: |-
        This API endpoint allows you to rename your server.

        The input is expected to be in JSON or XML format in the body parameter of the PUT request. The exact
        schema is defined below. Any extra parameters passed in the body will be ignored.
      operationId: putServers.Format
      x-api-path-slug: serversid-format-put
      parameters:
      - in: path
        name: id
        description: Server ID
        type: integer
      - in: body
        name: server
        description: New name of the server
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Servers
      - ""
      - .
      - Format
    delete:
      summary: Delete Servers  . Format
      description: |-
        This API endpoint deletes a server and all of its reported data.

        WARNING: Only servers that have stopped reporting can be deleted. This is an irreversible process which
        will delete all reported data for this server.
      operationId: deleteServers.Format
      x-api-path-slug: serversid-format-delete
      parameters:
      - in: path
        name: id
        description: Server ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Servers
      - ""
      - .
      - Format
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