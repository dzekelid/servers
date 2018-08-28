---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Get Servers. Format
  version: 1.0.0
  description: |-
    This API endpoint returns a paginated
    list of the Servers associated with your New Relic account. The time range for summary data is the last 10 minutes.

    Servers can be filtered by their name, hostname, or the list of server IDs.

    See our documentation for a discussion and examples of
    using filters
    and summary data output.
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
  /alerts_entity_conditions/{entity_id}.{format}:
    get:
      summary: Get Alerts Entity Conditions Entity  . Format
      description: |-
        This API endpoint allows you to list the Alerts conditions an entity is part of.

        Entity type options (Synthetics is not yet supported):

        BrowserApplication

        Application

        MobileApplication

        Server

        KeyTransaction

        Plugin
      operationId: getAlertsEntityConditionsEntity.Format
      x-api-path-slug: alerts-entity-conditionsentity-id-format-get
      parameters:
      - in: path
        name: entity_id
        description: Entity ID
        type: integer
      - in: query
        name: entity_type
        description: Entity Type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Entity
      - Conditions
      - Entity
      - ""
      - .
      - Format
    put:
      summary: Put Alerts Entity Conditions Entity  . Format
      description: "This API endpoint allows you to add an entity to a specified Alerts
        condition.\n\nNote: Admin User???s API Key is required.\n \n  Entity type
        options (Synthetics is not yet supported):\n\nBrowserApplication\n\nApplication\n\nMobileApplication\n\nServer\n\nKeyTransaction\n\nPlugin"
      operationId: putAlertsEntityConditionsEntity.Format
      x-api-path-slug: alerts-entity-conditionsentity-id-format-put
      parameters:
      - in: query
        name: condition_id
        description: Alerts condition ID
        type: integer
      - in: path
        name: entity_id
        description: Entity id to add
        type: integer
      - in: query
        name: entity_type
        description: Entity Type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Entity
      - Conditions
      - Entity
      - ""
      - .
      - Format
    delete:
      summary: Delete Alerts Entity Conditions Entity  . Format
      description: |-
        This API endpoint allows you to disassociate an entity with a specified Alerts condition.

        Note: Admin User???s API Key is required.

        Entity type options (Synthetics is not yet supported):

        BrowserApplication

        Application

        MobileApplication

        Server

        KeyTransaction

        Plugin
      operationId: deleteAlertsEntityConditionsEntity.Format
      x-api-path-slug: alerts-entity-conditionsentity-id-format-delete
      parameters:
      - in: query
        name: condition_id
        description: Alerts condition ID
        type: integer
      - in: path
        name: entity_id
        description: Entity id to remove
        type: integer
      - in: query
        name: entity_type
        description: Entity Type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Entity
      - Conditions
      - Entity
      - ""
      - .
      - Format
  /alerts_events.{format}:
    get:
      summary: Get Alerts Events. Format
      description: "This API endpoint allows you to list the alert events for your
        account.\n\nAlerts events can be filter by product, target type, group ID,
        instance ID, and event type.\n\nThe options for products are: APM, BROWSER,
        MOBILE, SERVERS, PLUGINS, SYNTHETICS, and ALERTS.\n\nThe options for entity
        type are: Application, Server, KeyTransaction, Plugin, MobileApplication,
        BrowserApplication, and Monitor.\n\nThe options for event type are: NOTIFICATION,
        DEPLOYMENT, VIOLATION_OPEN, VIOLATION_CLOSE, VIOLATION, and INSTRUMENTATION.\n\nThe
        group ID option is normally the same as the entity ID (e.g. an Application
        group ID and entity ID will be the same), however PLUGINS have a group ID
        representing the PLUGIN itself, and entity IDs for all instances of that PLUGIN
        type.\n\nSee our documentation for a discussion on \noutput pagination."
      operationId: getAlertsEvents.Format
      x-api-path-slug: alerts-events-format-get
      parameters:
      - in: query
        name: filter[entity_group_id]
        description: Filter by entity group ID
        type: integer
      - in: query
        name: filter[entity_id]
        description: Filter by entity ID
        type: integer
      - in: query
        name: filter[entity_type]
        description: Filter by entity type
        type: string
      - in: query
        name: filter[event_type]
        description: Filter by event type
        type: string
      - in: query
        name: filter[product]
        description: Filter by New Relic product
        type: string
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Events.
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