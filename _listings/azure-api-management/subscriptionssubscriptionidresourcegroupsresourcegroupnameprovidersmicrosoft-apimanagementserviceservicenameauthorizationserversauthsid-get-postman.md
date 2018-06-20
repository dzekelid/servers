{
  "info": {
    "name": "Azure API Management API AuthorizationServers Get",
    "_postman_id": "ab30d24d-3a83-4d17-84ec-f5fce1bdb7f0",
    "description": "Gets the details of the authorization server specified by its identifier.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "authorization servers",
      "item": [
        {
          "id": "ce188683-bd8a-4390-86d9-5689fb0944f1",
          "name": "AuthorizationServers_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ApiManagement/service/:serviceName/authorizationServers/:authsid"
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
                  "id": "serviceName",
                  "value": "serviceName",
                  "type": "string"
                },
                {
                  "id": "authsid",
                  "value": "authsid",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the details of the authorization server specified by its identifier"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1732b98-bb2d-468e-be23-e1d76c01b089"
            }
          ]
        }
      ]
    }
  ]
}