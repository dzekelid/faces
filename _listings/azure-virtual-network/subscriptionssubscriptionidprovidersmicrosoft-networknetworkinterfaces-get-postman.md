{
  "info": {
    "name": "Azure Virtual Network API Network Interfaces List All",
    "_postman_id": "cc8a1008-bbf7-4c42-b73d-97457dd9c59c",
    "description": "Gets all network interfaces in a subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "network interfaces",
      "item": [
        {
          "id": "d4da6fbf-b6ad-44fd-a761-90978c8e5ba1",
          "name": "NetworkInterfaces_ListAll",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Network/networkInterfaces"
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
            "description": "Gets all network interfaces in a subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "beee9b95-fd0e-4ba5-9e2a-9efe81637489"
            }
          ]
        }
      ]
    }
  ]
}