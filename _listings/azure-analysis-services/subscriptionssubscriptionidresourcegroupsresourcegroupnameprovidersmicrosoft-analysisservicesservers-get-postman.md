{
  "info": {
    "name": "Azure Analysis Services API List Servers By Group",
    "_postman_id": "fcfd010f-1b37-49e3-b97d-2cd7763f722b",
    "description": "Gets all the Analysis Services servers for the given resource group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "servers",
      "item": [
        {
          "id": "0eb680a6-cf4a-4cf7-9960-9275e0c1cc20",
          "name": "Servers_ListByResourceGroup",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.AnalysisServices/servers"
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
            "description": "Gets all the Analysis Services servers for the given resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ce6c4bc-79ca-46af-bae1-625be8e5ba59"
            }
          ]
        }
      ]
    }
  ]
}