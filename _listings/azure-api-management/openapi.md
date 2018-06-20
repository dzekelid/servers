---
swagger: "2.0"
x-collection-name: Azure API Management
x-complete: 1
info:
  title: ApiManagementClient
  description: use-these-rest-apis-for-performing-operations-on-user-entity-in-azure-api-management-deployment--the-user-entity-in-api-management-represents-the-developers-that-call-the-apis-of-the-products-to-which-they-are-subscribed-
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/authorizationServers
  : get:
      summary: AuthorizationServers ListByService
      description: Lists a collection of authorization servers defined within a service
        instance.
      operationId: AuthorizationServers_ListByService
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameauthorizationservers-get
      parameters:
      - in: query
        name: $filter
        description: '| Field | Supported operators    | Supported functions                         ||-------|------------------------|---------------------------------------------||
          id    | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith
          || name  | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith
          |'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Authorization Servers
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/authorizationServers/{authsid}
  : get:
      summary: AuthorizationServers Get
      description: Gets the details of the authorization server specified by its identifier.
      operationId: AuthorizationServers_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameauthorizationserversauthsid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Authorization Servers
    put:
      summary: AuthorizationServers CreateOrUpdate
      description: Creates new authorization server or updates an existing authorization
        server.
      operationId: AuthorizationServers_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameauthorizationserversauthsid-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Create or update parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Authorization Servers
    patch:
      summary: AuthorizationServers Update
      description: Updates the details of the authorization server specified by its
        identifier.
      operationId: AuthorizationServers_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameauthorizationserversauthsid-patch
      parameters:
      - in: header
        name: If-Match
        description: The entity state (Etag) version of the authorization server to
          update
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: OAuth2 Server settings Update parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Authorization Servers
    delete:
      summary: AuthorizationServers Delete
      description: Deletes specific authorization server instance.
      operationId: AuthorizationServers_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenameauthorizationserversauthsid-delete
      parameters:
      - in: header
        name: If-Match
        description: The entity state (Etag) version of the authentication server
          to delete
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Authorization Servers
---