{
  "info": {
    "name": "Azure SQL Database API Servers Get Service Objective",
    "_postman_id": "6ce77438-00fc-4c93-89b8-e90b72d852f8",
    "description": "Gets a database service objective.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "servers service objective",
      "item": [
        {
          "id": "1d40561e-b642-4da0-b52d-5ce226fe9432",
          "name": "Servers_GetServiceObjective",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/serviceObjectives/:serviceObjectiveName"
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
                  "id": "serviceObjectiveName",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Gets a database service objective"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aebd8712-94df-484b-9f03-5c246855f5b5"
            }
          ]
        }
      ]
    }
  ]
}