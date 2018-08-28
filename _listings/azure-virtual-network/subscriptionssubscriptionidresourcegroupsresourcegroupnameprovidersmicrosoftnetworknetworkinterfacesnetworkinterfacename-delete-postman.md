{
  "info": {
    "name": "Azure Virtual Network API Network Interfaces Delete",
    "_postman_id": "98725cda-7ad2-42a4-9b71-3fcdaad9e475",
    "description": "Deletes the specified network interface.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "network interfaces",
      "item": [
        {
          "id": "3ad246b4-f514-4e89-adf9-ce52d4a1b672",
          "name": "NetworkInterfaces_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Network/networkInterfaces/:networkInterfaceName"
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
                  "id": "networkInterfaceName",
                  "value": "{}",
                  "type": "string"
                },
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified network interface"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff3b234f-ef5e-4ed3-8daf-b9e3fdda3d08"
            }
          ]
        }
      ]
    }
  ]
}