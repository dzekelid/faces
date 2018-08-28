---
swagger: "2.0"
x-collection-name: Azure Virtual Network
x-complete: 0
info:
  title: Azure Virtual Network API Network Interfaces List Virtual Machine Scale Set
    Network Interfaces
  description: Gets all network interfaces in a virtual machine scale set.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/networkInterfaces/{networkInterfaceName}
  : delete:
      summary: Network Interfaces Delete
      description: Deletes the specified network interface.
      operationId: NetworkInterfaces_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networknetworkinterfacesnetworkinterfacename-delete
      parameters:
      - in: path
        name: networkInterfaceName
        description: The name of the network interface
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Network Interfaces
    get:
      summary: Network Interfaces Get
      description: Gets information about the specified network interface.
      operationId: NetworkInterfaces_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networknetworkinterfacesnetworkinterfacename-get
      parameters:
      - in: query
        name: $expand
        description: Expands referenced resources
      - in: path
        name: networkInterfaceName
        description: The name of the network interface
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Network Interfaces
    put:
      summary: Network Interfaces Create Or Update
      description: Creates or updates a network interface.
      operationId: NetworkInterfaces_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networknetworkinterfacesnetworkinterfacename-put
      parameters:
      - in: path
        name: networkInterfaceName
        description: The name of the network interface
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to the create or update network interface
          operation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Network Interfaces
  /subscriptions/{subscriptionId}/providers/Microsoft.Network/networkInterfaces:
    get:
      summary: Network Interfaces List All
      description: Gets all network interfaces in a subscription.
      operationId: NetworkInterfaces_ListAll
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-networknetworkinterfaces-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Network Interfaces
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/networkInterfaces:
    get:
      summary: Network Interfaces List
      description: Gets all network interfaces in a resource group.
      operationId: NetworkInterfaces_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networknetworkinterfaces-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Network Interfaces
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/networkInterfaces/{networkInterfaceName}/effectiveRouteTable
  : post:
      summary: Network Interfaces Get Effective Route Table
      description: Gets all route tables applied to a network interface.
      operationId: NetworkInterfaces_GetEffectiveRouteTable
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networknetworkinterfacesnetworkinterfacenameeffectiveroutetable-post
      parameters:
      - in: path
        name: networkInterfaceName
        description: The name of the network interface
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Network Interfaces
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/networkInterfaces/{networkInterfaceName}/effectiveNetworkSecurityGroups
  : post:
      summary: Network Interfaces List Effective Network Security Groups
      description: Gets all network security groups applied to a network interface.
      operationId: NetworkInterfaces_ListEffectiveNetworkSecurityGroups
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-networknetworkinterfacesnetworkinterfacenameeffectivenetworksecuritygroups-post
      parameters:
      - in: path
        name: networkInterfaceName
        description: The name of the network interface
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Network Interfaces
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.Compute/virtualMachineScaleSets/{virtualMachineScaleSetName}/virtualMachines/{virtualmachineIndex}/networkInterfaces
  : get:
      summary: Network Interfaces List Virtual Machine Scale Set VMNetwork Interfaces
      description: Gets information about all network interfaces in a virtual machine
        in a virtual machine scale set.
      operationId: NetworkInterfaces_ListVirtualMachineScaleSetVMNetworkInterfaces
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-computevirtualmachinescalesetsvirtualmachinescalesetnamevirtualmachinesvirtualmachineindexnetworkinterfaces-get
      parameters:
      - in: query
        name: api-version
        description: Client API version
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: virtualmachineIndex
        description: The virtual machine index
      - in: path
        name: virtualMachineScaleSetName
        description: The name of the virtual machine scale set
      responses:
        200:
          description: OK
      tags:
      - Network Interfaces
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.Compute/virtualMachineScaleSets/{virtualMachineScaleSetName}/networkInterfaces
  : get:
      summary: Network Interfaces List Virtual Machine Scale Set Network Interfaces
      description: Gets all network interfaces in a virtual machine scale set.
      operationId: NetworkInterfaces_ListVirtualMachineScaleSetNetworkInterfaces
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-computevirtualmachinescalesetsvirtualmachinescalesetnamenetworkinterfaces-get
      parameters:
      - in: query
        name: api-version
        description: Client API version
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: virtualMachineScaleSetName
        description: The name of the virtual machine scale set
      responses:
        200:
          description: OK
      tags:
      - Network Interfaces
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---