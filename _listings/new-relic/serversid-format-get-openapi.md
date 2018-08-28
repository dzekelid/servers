---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Get Servers  . Format
  version: 1.0.0
  description: |-
    This API endpoint returns a single Server, identified by ID. The time range for summary data is the last 10 minutes.???

    See our documentation for a discussion on
    summary data output.
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