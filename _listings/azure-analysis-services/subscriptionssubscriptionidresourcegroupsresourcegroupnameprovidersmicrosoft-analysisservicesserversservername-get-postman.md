{
  "info": {
    "name": "Azure Analysis Services API Get Server",
    "_postman_id": "6d1376dc-3155-4bd4-9823-60cab6b18121",
    "description": "Gets details about the specified Analysis Services server.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "servers",
      "item": [
        {
          "id": "d42d20af-484c-4eda-bb6f-493ca22dfca8",
          "name": "Servers_GetDetails",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets details about the specified Analysis Services server"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc7e3e24-2872-4adf-b0f6-c7ebdccfbb3c"
            }
          ]
        }
      ]
    }
  ]
}