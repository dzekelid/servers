swagger: "2.0"
x-collection-name: Azure SQL Database
x-complete: 1
info:
  title: Azure SQL Database
  description: provides-create-read-update-and-delete-functionality-for-azure-sql-database-resources-including-servers-databases-elastic-pools-recommendations-operations-and-usage-metrics-
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/providers/Microsoft.Sql/servers:
    get:
      summary: Servers List
      description: Returns a list of servers.
      operationId: Servers_List
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-sqlservers-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Servers
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}:
    put:
      summary: Servers Create Or Update
      description: Creates or updates a new server.
      operationId: Servers_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservername-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The required parameters for creating or updating a server
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Servers
    delete:
      summary: Servers Delete
      description: Deletes a SQL server.
      operationId: Servers_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservername-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Servers
    get:
      summary: Servers Get
      description: Gets a server.
      operationId: Servers_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservername-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Servers
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers:
    get:
      summary: Servers List By Resource Group
      description: Returns a list of servers in a resource group.
      operationId: Servers_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlservers-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Servers Resource Group
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/serviceObjectives/{serviceObjectiveName}
  : get:
      summary: Servers Get Service Objective
      description: Gets a database service objective.
      operationId: Servers_GetServiceObjective
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameserviceobjectivesserviceobjectivename-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: serviceObjectiveName
        description: The name of the service objective to retrieve
      responses:
        200:
          description: OK
      tags:
      - Servers Service Objective
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/serviceObjectives
  : get:
      summary: Servers List Service Objectives
      description: Returns database service objectives.
      operationId: Servers_ListServiceObjectives
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameserviceobjectives-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Servers Service Objectives
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/usages:
    get:
      summary: Servers List Usages
      description: Returns server usages.
      operationId: Servers_ListUsages
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameusages-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Servers Usages