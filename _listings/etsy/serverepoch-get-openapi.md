---
swagger: "2.0"
x-collection-name: Etsy
x-complete: 0
info:
  title: Etsy Get Server Epoch
  description: Get server time, in epoch seconds notation.
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /server/epoch:
    get:
      summary: Get Server Epoch
      description: Get server time, in epoch seconds notation.
      operationId: getServerEpoch
      x-api-path-slug: serverepoch-get
      responses:
        200:
          description: OK
      tags:
      - Server
      - Epoch
  /server/ping:
    get:
      summary: Get Server Ping
      description: Check that the server is alive.
      operationId: getServerPing
      x-api-path-slug: serverping-get
      responses:
        200:
          description: OK
      tags:
      - Server
      - Ping
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