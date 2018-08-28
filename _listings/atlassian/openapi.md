swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/serverInfo:
    get:
      summary: Get server info
      description: Returns general information about the current Jira server.
      operationId: com.atlassian.jira.rest.v2.ServerInfoResource.getServerInfo_get
      x-api-path-slug: api2serverinfo-get
      responses:
        200:
          description: OK
      tags:
      - Server
      - Info