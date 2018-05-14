{
  "info": {
    "name": "Azure SQL Database API Servers List Usages",
    "_postman_id": "de44c1c2-58fe-4f64-bc4e-5e28389e4f12",
    "description": "Returns server usages.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "servers usages",
      "item": [
        {
          "id": "23e78e75-72e5-47cb-b66f-d7eb1f33284f",
          "name": "Servers_ListUsages",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/usages"
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
            "description": "Returns server usages"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "374070fc-9481-4d4c-be9f-409e5f3dae9e"
            }
          ]
        }
      ]
    }
  ]
}