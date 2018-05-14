{
  "info": {
    "name": "Azure Analysis Services API Delete Servers",
    "_postman_id": "68db2aeb-d992-4cbf-bd79-77c224511b76",
    "description": "Deletes the specified Analysis Services server.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "servers",
      "item": [
        {
          "id": "f1673763-feb9-4242-bb10-a15245b47aac",
          "name": "Servers_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.AnalysisServices/servers/:serverName"
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
                  "id": "serverName",
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
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Analysis Services server"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5833a60a-a15d-4870-a757-d602f08d2c1a"
            }
          ]
        }
      ]
    }
  ]
}