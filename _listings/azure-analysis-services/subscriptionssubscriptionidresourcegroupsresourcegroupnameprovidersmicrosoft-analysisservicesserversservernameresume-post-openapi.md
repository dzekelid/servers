---
swagger: "2.0"
x-collection-name: Azure Analysis Services
x-complete: 0
info:
  title: Azure Analysis Services API Resume Server
  description: Resumes operation of the specified Analysis Services server instance.
  version: "2016-05-16"
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.AnalysisServices/servers/{serverName}:
    get:
      summary: Get Server
      description: Gets details about the specified Analysis Services server.
      operationId: Servers_GetDetails
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-analysisservicesserversservername-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: serverName
        description: The name of the Analysis Services server
      responses:
        200:
          description: OK
      tags:
      - Servers
    put:
      summary: Create Server
      description: Provisions the specified Analysis Services server based on the
        configuration specified in the request.
      operationId: Servers_Create
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-analysisservicesserversservername-put
      parameters:
      - in: query
        name: No Name
      - in: path
        name: serverName
        description: The name of the Analysis Services server
      - in: body
        name: serverParameters
        description: Contains the information used to provision the Analysis Services
          server
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Servers
    delete:
      summary: Delete Servers
      description: Deletes the specified Analysis Services server.
      operationId: Servers_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-analysisservicesserversservername-delete
      parameters:
      - in: query
        name: No Name
      - in: path
        name: serverName
        description: The name of the Analysis Services server
      responses:
        200:
          description: OK
      tags:
      - Servers
    patch:
      summary: Update Server
      description: Updates the current state of the specified Analysis Services server.
      operationId: Servers_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-analysisservicesserversservername-patch
      parameters:
      - in: query
        name: No Name
      - in: path
        name: serverName
        description: The name of the Analysis Services server
      - in: body
        name: serverUpdateParameters
        description: Request object that contains the updated information for the
          server
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Servers
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.AnalysisServices/servers/{serverName}/suspend
  : post:
      summary: Suspend Server
      description: Supends operation of the specified Analysis Services server instance.
      operationId: Servers_Suspend
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-analysisservicesserversservernamesuspend-post
      parameters:
      - in: query
        name: No Name
      - in: path
        name: serverName
        description: The name of the Analysis Services server
      responses:
        200:
          description: OK
      tags:
      - Servers
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.AnalysisServices/servers/{serverName}/resume
  : post:
      summary: Resume Server
      description: Resumes operation of the specified Analysis Services server instance.
      operationId: Servers_Resume
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-analysisservicesserversservernameresume-post
      parameters:
      - in: query
        name: No Name
      - in: path
        name: serverName
        description: The name of the Analysis Services server
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