{
  "info": {
    "name": "Azure Analysis Services API Resume Server",
    "_postman_id": "a1644941-0248-4eb5-8715-2e191c020480",
    "description": "Resumes operation of the specified Analysis Services server instance.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "servers",
      "item": [
        {
          "id": "cab5ba49-f17d-4ac4-94b9-bfa21c5e8884",
          "name": "Servers_Resume",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.AnalysisServices/servers/:serverName/resume"
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
            "description": "Resumes operation of the specified Analysis Services server instance"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "372ab7b7-f1b2-46c2-81df-2d2b2f044ab0"
            }
          ]
        }
      ]
    }
  ]
}