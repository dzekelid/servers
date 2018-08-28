---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix SAS ESP Predix Service ESP server health check
  description: API to to check health of ESP server.
  contact:
    name: zahid.iqbal2@ge.com
  version: 1.0.0
host: sas-proxy.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/proxy/server:
    head:
      summary: ESP server health check
      description: API to to check health of ESP server.
      operationId: healthCheckUsingHEAD
      x-api-path-slug: v1proxyserver-head
      parameters:
      - in: body
        name: reqBody
        description: reqBody
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - ESP
      - Server
      - Health
      - Check
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