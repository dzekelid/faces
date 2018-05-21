---
swagger: "2.0"
x-collection-name: Azure Virtual Network
x-complete: 1
info:
  title: NetworkManagementClient
  description: the-microsoft-azure-network-management-api-provides-a-restful-set-of-web-services-that-interact-with-microsoft-azure-networks-service-to-manage-your-network-resources-the-api-has-entities-that-capture-the-relationship-between-an-end-user-and-the-microsoft-azure-networks-service
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftnetworknetworkinterfacesnetworkinterfacename-delete
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftnetworknetworkinterfacesnetworkinterfacename-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftnetworknetworkinterfacesnetworkinterfacename-put
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
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftnetworknetworkinterfaces-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftnetworknetworkinterfaces-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftnetworknetworkinterfacesnetworkinterfacenameeffectiveroutetable-post
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftnetworknetworkinterfacesnetworkinterfacenameeffectivenetworksecuritygroups-post
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftcomputevirtualmachinescalesetsvirtualmachinescalesetnamevirtualmachinesvirtualmachineindexnetworkinterfaces-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftcomputevirtualmachinescalesetsvirtualmachinescalesetnamenetworkinterfaces-get
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.Compute/virtualMachineScaleSets/{virtualMachineScaleSetName}/virtualMachines/{virtualmachineIndex}/networkInterfaces/{networkInterfaceName}
  : get:
      summary: Network Interfaces Get Virtual Machine Scale Set Network Interface
      description: Get the specified network interface in a virtual machine scale
        set.
      operationId: NetworkInterfaces_GetVirtualMachineScaleSetNetworkInterface
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftcomputevirtualmachinescalesetsvirtualmachinescalesetnamevirtualmachinesvirtualmachineindexnetworkinterfacesnetworkinterfacename-get
      parameters:
      - in: query
        name: $expand
        description: Expands referenced resources
      - in: query
        name: api-version
        description: Client API version
      - in: path
        name: networkInterfaceName
        description: The name of the network interface
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
---