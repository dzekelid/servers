{
  "info": {
    "name": "Azure API Management API AuthorizationServers Delete",
    "_postman_id": "f30a5430-7485-466b-a268-94ebbc22271a",
    "description": "Deletes specific authorization server instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "authorization servers",
      "item": [
        {
          "id": "b88ed423-e3f8-40c2-a018-bd1820af3a7e",
          "name": "AuthorizationServers_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ApiManagement/service/:serviceName/authorizationServers/:authsid"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                },
                {
                  "id": "serviceName",
                  "value": "serviceName",
                  "type": "string"
                },
                {
                  "id": "authsid",
                  "value": "authsid",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "If-Match",
                "value": "{}",
                "description": "The entity state (Etag) version of the authentication server to delete",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes specific authorization server instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01e15796-5f34-42d2-91b6-f725f3a2da6f"
            }
          ]
        }
      ]
    }
  ]
}