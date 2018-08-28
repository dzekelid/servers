---
swagger: "2.0"
x-collection-name: Hewlett Packard Enterprise (HPE)
x-complete: 0
info:
  title: HPE OneSphere API Get Servers
  description: Returns servers.
  termsOfService: http://www.hpe.com/onesphere
  contact:
    name: HPE OneSphere API team
    url: http://www.hpe.com/onesphere
  version: 1.0.0
host: deic02-hpe.hpeonesphere.com
basePath: /rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /servers:
    get:
      summary: Get Servers
      description: Returns servers.
      operationId: GetServer
      x-api-path-slug: servers-get
      parameters:
      - in: query
        name: applianceUri
        description: Set of servers in this appliance
      - in: query
        name: regionUri
        description: Set of servers in this region
      - in: query
        name: zoneUri
        description: Set of servers in this zone
      responses:
        200:
          description: OK
      tags:
      - Servers
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