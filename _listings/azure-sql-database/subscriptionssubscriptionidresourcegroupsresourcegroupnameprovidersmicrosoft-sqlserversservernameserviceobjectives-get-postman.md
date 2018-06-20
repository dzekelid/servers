{
  "info": {
    "name": "Azure SQL Database API Servers List Service Objectives",
    "_postman_id": "5c663909-17cd-44c6-bcd0-62dfd2f810f1",
    "description": "Returns database service objectives.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "servers service objectives",
      "item": [
        {
          "id": "435097bb-5fd7-4b5e-95b7-50fac97adb7b",
          "name": "Servers_ListServiceObjectives",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/serviceObjectives"
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
                  "id": "serverName",
                  "value": "serverName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns database service objectives"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ce68b0a-db15-4a85-8a6d-483fb59e6410"
            }
          ]
        }
      ]
    }
  ]
}