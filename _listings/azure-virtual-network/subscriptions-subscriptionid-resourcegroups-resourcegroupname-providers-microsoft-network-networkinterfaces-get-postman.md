{
  "info": {
    "name": "Azure Virtual Network API Network Interfaces List",
    "_postman_id": "da33d28f-1025-4791-8347-3c243d7deeb6",
    "description": "Gets all network interfaces in a resource group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "network interfaces",
      "item": [
        {
          "id": "eb8d61f1-6e22-450f-8b34-523ca602fa8b",
          "name": "NetworkInterfaces_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Network/networkInterfaces"
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
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Gets all network interfaces in a resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03343d9f-ce40-478c-accf-b7d44f3501de"
            }
          ]
        }
      ]
    }
  ]
}