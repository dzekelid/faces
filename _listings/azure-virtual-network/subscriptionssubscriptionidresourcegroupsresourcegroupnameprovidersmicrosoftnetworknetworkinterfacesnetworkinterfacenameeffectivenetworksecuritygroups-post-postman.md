{
  "info": {
    "name": "Azure Virtual Network API Network Interfaces List Effective Network Security Groups",
    "_postman_id": "87c6646f-67c5-4279-9437-c2e86ad14fca",
    "description": "Gets all network security groups applied to a network interface.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "network interfaces",
      "item": [
        {
          "id": "2b9ea94e-66be-4b02-a431-6c48b5c7fd8e",
          "name": "NetworkInterfaces_ListEffectiveNetworkSecurityGroups",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Network/networkInterfaces/:networkInterfaceName/effectiveNetworkSecurityGroups"
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all network security groups applied to a network interface"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0562cb1-b370-44ec-912a-a6a7d699863b"
            }
          ]
        }
      ]
    }
  ]
}