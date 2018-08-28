{
  "info": {
    "name": "Azure SQL Database API Servers List",
    "_postman_id": "3011c7b3-1519-4e83-b603-35157cd8955f",
    "description": "Returns a list of servers.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "servers",
      "item": [
        {
          "id": "d578172a-5b60-46d1-948f-c0136cf59663",
          "name": "Servers_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Sql/servers"
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of servers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7da412df-bb7a-485c-a5a8-bf18b8b38433"
            }
          ]
        }
      ]
    }
  ]
}