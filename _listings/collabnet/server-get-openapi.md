---
swagger: "2.0"
x-collection-name: CollabNet
x-complete: 0
info:
  title: CollabNet TeamForge API Documentation Gets TeamForge server information
  version: 1.0.0
  description: Gets teamforge server information.
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /server:
    get:
      summary: Gets TeamForge server information
      description: Gets teamforge server information.
      operationId: getTeamForgeServerInfo
      x-api-path-slug: server-get
      responses:
        200:
          description: OK
      tags:
      - TeamForge
      - Server
      - Information
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