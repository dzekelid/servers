{
  "info": {
    "name": "Azure SQL Database API Servers List By Resource Group",
    "_postman_id": "6d1104ae-e210-4841-85b8-914daba2da94",
    "description": "Returns a list of servers in a resource group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "servers resource group",
      "item": [
        {
          "id": "fa62bbda-27f0-4cc0-b7f6-958e4e847a2b",
          "name": "Servers_ListByResourceGroup",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers"
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of servers in a resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e57d2e7e-d129-4cf7-b90c-c85487a6571b"
            }
          ]
        }
      ]
    }
  ]
}