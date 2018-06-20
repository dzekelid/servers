---
swagger: "2.0"
x-collection-name: AWS Server Migration Service
x-complete: 1
info:
  title: AWS Server Migration Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetServers:
    get:
      summary: Get Servers
      description: The get-servers API returns a list of all servers in your server
        catalog.
      operationId: getServers
      x-api-path-slug: actiongetservers-get
      parameters:
      - in: query
        name: maxResults
        description: 'Type: Integer'
        type: string
      - in: query
        name: nextToken
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Servers
---