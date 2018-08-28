{
  "info": {
    "name": "Azure SQL Database API Servers Delete",
    "_postman_id": "3a368d45-bded-4d1a-bc82-2f9e3b927833",
    "description": "Deletes a SQL server.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "servers",
      "item": [
        {
          "id": "b9a2de67-03ad-4776-ae24-fd1c9b6d6fc7",
          "name": "Servers_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName"
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a SQL server"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e41211ab-a990-4980-9b37-9cb880acfeec"
            }
          ]
        }
      ]
    }
  ]
}