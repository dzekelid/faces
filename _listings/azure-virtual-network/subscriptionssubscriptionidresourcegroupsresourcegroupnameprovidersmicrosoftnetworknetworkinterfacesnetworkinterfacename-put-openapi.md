---
swagger: "2.0"
x-collection-name: Azure Virtual Network
x-complete: 0
info:
  title: Azure Virtual Network API Network Interfaces Create Or Update
  description: Creates or updates a network interface.
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