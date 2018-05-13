{
  "info": {
    "name": "Azure Virtual Network API Network Interfaces List Virtual Machine Scale Set Network Interfaces",
    "_postman_id": "696e0893-b25e-4e8e-98b8-35c95fc55615",
    "description": "Gets all network interfaces in a virtual machine scale set.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "network interfaces",
      "item": [
        {
          "id": "e0991a01-3aef-4aad-89fc-1a41a10ccb86",
          "name": "NetworkInterfaces_ListVirtualMachineScaleSetNetworkInterfaces",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/microsoft.Compute/virtualMachineScaleSets/:virtualMachineScaleSetName/networkInterfaces"
              ],
              "query": [
                {
                  "key": "api-version",
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
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "virtualMachineScaleSetName",
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
            "description": "Gets all network interfaces in a virtual machine scale set"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35f1b1e2-546f-47e8-900e-09c843fae239"
            }
          ]
        }
      ]
    }
  ]
}