{
  "info": {
    "name": "Azure Virtual Network API Network Interfaces Get Effective Route Table",
    "_postman_id": "a328f74d-bea7-43bc-bb7f-36a58ffe952c",
    "description": "Gets all route tables applied to a network interface.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "network interfaces",
      "item": [
        {
          "id": "29059a1f-9f0f-47de-b721-71fac527f160",
          "name": "NetworkInterfaces_GetEffectiveRouteTable",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Network/networkInterfaces/:networkInterfaceName/effectiveRouteTable"
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
            "description": "Gets all route tables applied to a network interface"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ee831f2-7512-4cf8-b427-1d66fd7a7d54"
            }
          ]
        }
      ]
    }
  ]
}