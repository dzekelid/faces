{
  "info": {
    "name": "Azure Virtual Network API Network Interfaces List Virtual Machine Scale Set VMNetwork Interfaces",
    "_postman_id": "21bfa2db-cfa3-4af8-b5e3-750066cc2230",
    "description": "Gets information about all network interfaces in a virtual machine in a virtual machine scale set.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "network interfaces",
      "item": [
        {
          "id": "58db1dcc-ab36-401e-80cb-6adfaa78bee6",
          "name": "NetworkInterfaces_ListVirtualMachineScaleSetVMNetworkInterfaces",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/microsoft.Compute/virtualMachineScaleSets/:virtualMachineScaleSetName/virtualMachines/:virtualmachineIndex/networkInterfaces"
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
                  "id": "virtualmachineIndex",
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
            "description": "Gets information about all network interfaces in a virtual machine in a virtual machine scale set"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34f57835-20ff-403f-91f0-87d86b78f583"
            }
          ]
        }
      ]
    }
  ]
}