{
  "info": {
    "name": "Azure API Management API AuthorizationServers ListByService",
    "_postman_id": "7cd5aaa2-6728-4363-b32a-e85e9323efe4",
    "description": "Lists a collection of authorization servers defined within a service instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "authorization servers",
      "item": [
        {
          "id": "f798fd67-f7c9-48ae-b25a-8f93c4a4d81a",
          "name": "AuthorizationServers_ListByService",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ApiManagement/service/:serviceName/authorizationServers"
              ],
              "query": [
                {
                  "key": "$filter",
                  "value": "%7B%7D",
                  "disabled": false
                },
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists a collection of authorization servers defined within a service instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69e29aca-e4d5-4505-a6de-02d8e17a47b6"
            }
          ]
        }
      ]
    }
  ]
}