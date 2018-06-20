---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Get Servers Server  Metrics Data. Format
  version: 1.0.0
  description: "This API endpoint returns a list of values for each of the requested
    metrics. The list of available metrics\ncan be returned using the Metric Name
    API endpoint.\n\nMetric data can be filtered by a number of parameters, including
    multiple names and values, and by time range.\nMetric names and values will be
    matched intelligently in the background.\n\nYou can also retrieve a summarized
    data point across the entire time range selected by using the summarize\nparameter.\n\nSee
    our documentation for a discussion on \noutput pagination,  time range \nrelated
    considerations, and for examples of requesting and using metric values."
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
  /servers/{server_id}/metrics.{format}:
    get:
      summary: Get Servers Server  Metrics. Format
      description: |-
        Return a list of known metrics and their value names for the given resource.

        See our documentation for a discussion
        on  output pagination
        and for examples of requesting and using metric values.
      operationId: getServersServerMetrics.Format
      x-api-path-slug: serversserver-idmetrics-format-get
      parameters:
      - in: query
        name: cursor
        description: Cursor for next page (replacing page param)
        type: string
      - in: query
        name: name
        description: Filter metrics by name
        type: string
      - in: query
        name: page
        description: Pagination index (will be deprecated)
        type: integer
      - in: path
        name: server_id
        description: Server ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Servers
      - Server
      - ""
      - Metrics.
      - Format
  /servers/{server_id}/metrics/data.{format}:
    get:
      summary: Get Servers Server  Metrics Data. Format
      description: "This API endpoint returns a list of values for each of the requested
        metrics. The list of available metrics\ncan be returned using the Metric Name
        API endpoint.\n\nMetric data can be filtered by a number of parameters, including
        multiple names and values, and by time range.\nMetric names and values will
        be matched intelligently in the background.\n\nYou can also retrieve a summarized
        data point across the entire time range selected by using the summarize\nparameter.\n\nSee
        our documentation for a discussion on \noutput pagination,  time range \nrelated
        considerations, and for examples of requesting and using metric values."
      operationId: getServersServerMetricsData.Format
      x-api-path-slug: serversserver-idmetricsdata-format-get
      parameters:
      - in: query
        name: from
        description: Retrieve metrics after this time
        type: time
      - in: query
        name: names
        description: Retrieve specific metrics by name
        type: array
      - in: query
        name: period
        description: Period of timeslices in seconds
        type: integer
      - in: query
        name: raw
        description: Return unformatted raw values
        type: boolean
      - in: path
        name: server_id
        description: Server ID
        type: integer
      - in: query
        name: summarize
        description: Summarize the data
        type: boolean
      - in: query
        name: to
        description: Retrieve metrics before this time
        type: time
      - in: query
        name: values
        description: Retrieve specific metric values
        type: array
      responses:
        200:
          description: OK
      tags:
      - Servers
      - Server
      - ""
      - Metrics
      - Data.
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