---
swagger: "2.0"
x-collection-name: Google Container Engine
x-complete: 0
info:
  title: Google Container Engine API Get Server Configuration
  description: Returns configuration info about the Container Engine service.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: container.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/projects/{projectId}/zones/{zone}/serverconfig:
    get:
      summary: Get Server Configuration
      description: Returns configuration info about the Container Engine service.
      operationId: container.projects.zones.getServerconfig
      x-api-path-slug: v1projectsprojectidzoneszoneserverconfig-get
      parameters:
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://support
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          to return operations for
      responses:
        200:
          description: OK
      tags:
      - Server
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