{
  "info": {
    "name": "Azure Analysis Services API Suspend Server",
    "_postman_id": "c367e9cf-f5b0-4413-9e9f-4f1f6d0af8d9",
    "description": "Supends operation of the specified Analysis Services server instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "servers",
      "item": [
        {
          "id": "1ee38302-3d18-452c-ab0c-d47e72ceaec1",
          "name": "Servers_Suspend",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.AnalysisServices/servers/:serverName/suspend"
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Supends operation of the specified Analysis Services server instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61ae508b-60d0-480e-8299-525947ebd88f"
            }
          ]
        }
      ]
    }
  ]
}