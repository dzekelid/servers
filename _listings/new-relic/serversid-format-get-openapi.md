---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Get Servers  . Format
  version: 1.0.0
  description: "This API endpoint returns a single Server, identified by ID. The time
    range for summary data is the last 10 minutes.\u201D\n\nSee our documentation
    for a discussion on\nsummary data output."
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /servers.{format}:
    get:
      summary: Get Servers. Format
      description: |-
        This API endpoint returns a paginated
        list of the Servers associated with your New Relic account. The time range for summary data is the last 10 minutes.

        Servers can be filtered by their name, hostname, or the list of server IDs.

        See our documentation for a discussion and examples of
        using filters
        and summary data output.
      operationId: getServers.Format
      x-api-path-slug: servers-format-get
      parameters:
      - in: query
        name: filter[host]
        description: Filter by host
        type: string
      - in: query
        name: filter[ids]
        description: Filter by server IDs
        type: list
      - in: query
        name: filter[labels]
        description: Filter by server labels (beta)
        type: string
      - in: query
        name: filter[name]
        description: Filter by name
        type: string
      - in: query
        name: filter[reported]
        description: Filter by reported in last 10 hours
        type: boolean
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Servers.
      - Format
  /servers/{id}.{format}:
    get:
      summary: Get Servers  . Format
      description: "This API endpoint returns a single Server, identified by ID. The
        time range for summary data is the last 10 minutes.\u201D\n\nSee our documentation
        for a discussion on\nsummary data output."
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