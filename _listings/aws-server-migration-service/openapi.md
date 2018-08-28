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
  /?Action=DeleteServerCatalog:
    get:
      summary: Delete Server Catalog
      description: The delete-server-catalog API clears all servers from your server
        catalog.
      operationId: deleteServerCatalog
      x-api-path-slug: actiondeleteservercatalog-get
      responses:
        200:
          description: OK
      tags:
      - Server Catalog
  /?Action=ImportServerCatalog:
    get:
      summary: Import Server Catalog
      description: The import-server-catalog API is used to gather the complete list
        of on-premises servers on your premises.
      operationId: importServerCatalog
      x-api-path-slug: actionimportservercatalog-get
      responses:
        200:
          description: OK
      tags:
      - Server Catalog
  /?Action=DisassociateConnector:
    get:
      summary: Disassociate Connector
      description: The disassociate-connector API will disassociate a connector from
        the Server Migration Service, rendering it unavailable to support replication
        jobs.
      operationId: disassociateConnector
      x-api-path-slug: actiondisassociateconnector-get
      parameters:
      - in: query
        name: connectorId
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Connectors
  /?Action=GetConnectors:
    get:
      summary: Get Connectors
      description: The get-connectors API returns a list of connectors that are registered
        with the Server Migration Service.
      operationId: getConnectors
      x-api-path-slug: actiongetconnectors-get
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
      - Connectors