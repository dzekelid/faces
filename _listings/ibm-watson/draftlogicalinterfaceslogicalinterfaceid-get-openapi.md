---
swagger: "2.0"
x-collection-name: IBM Watson
x-complete: 0
info:
  title: IBM Watson IoT Platform Get a draft logical interface
  description: Retrieve the draft logical interface with the specified id.
  version: 1.0.0
basePath: /api/v0002
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /physicalinterfaces:
    get:
      summary: Query active phyiscal interfaces
      description: |-
        Physical interfaces are used to model the interfaces between physical
        devices and the Watson IoT Platform.  A physical interface references
        event types.  Devices that implement a physical interface publish these
        events to the platform.

        The event types are referenced via a mapping that maps an event id to
        the id of an event type.  The event id corresponds to the MQTT topic
        that the event is published to by a device.

        The **physicalinterfaces** endpoint returns the list of all of the
        active physical interfaces that have been defined for the organization
        in the Watson IoT Platform.  Various query parameters can be used to
        filter, sort and page through the list of active physical interfaces
        that are returned.
      operationId: physical-interfaces-are-used-to-model-the-interfaces-between-physicaldevices-and-the-watson-iot-plat
      x-api-path-slug: physicalinterfaces-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Physicalinterfaces
  /physicalinterfaces/{physicalInterfaceId}:
    get:
      summary: Get an active physical interface
      description: Retrieve the active physical interface with the specified id.
      operationId: retrieve-the-active-physical-interface-with-the-specified-id
      x-api-path-slug: physicalinterfacesphysicalinterfaceid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Physicalinterfaces
      - PhysicalInterfaceId
  /physicalinterfaces/{physicalInterfaceId}/events:
    get:
      summary: Get the list of event mappings
      description: |-
        Retrieve the list of event mappings for the active physical interface.
        Event mappings are keyed off of the event id specified in the MQTT topic
        that the inbound events are published to.
      operationId: retrieve-the-list-of-event-mappings-for-the-active-physical-interfaceevent-mappings-are-keyed-off-of
      x-api-path-slug: physicalinterfacesphysicalinterfaceidevents-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Physicalinterfaces
      - PhysicalInterfaceId
      - Events
  /draft/physicalinterfaces:
    get:
      summary: Query draft phyiscal interfaces
      description: "Physical interfaces are used to model the interfaces between physical\ndevices
        and the Watson IoT Platform.  A physical interface references\nevent types.
        \ Devices that implement a physical interface publish these\nevents to the
        platform.\n\nThe event types are referenced via a mapping that maps an event
        id to\nthe id of an event type.  The event id corresponds to the MQTT topic\nthat
        the event is published to by a device.\n\nThe **/draft/physicalinterfaces**
        endpoint returns the list of all of \nthe draft physical interfaces that have
        been defined for the\norganization in the Watson IoT Platform.  Various query
        parameters can\nbe used to filter, sort and page through the list of draft
        physical\ninterfaces that are returned."
      operationId: physical-interfaces-are-used-to-model-the-interfaces-between-physicaldevices-and-the-watson-iot-plat
      x-api-path-slug: draftphysicalinterfaces-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Physicalinterfaces
    post:
      summary: Create a draft physical interface
      description: "Creates a new draft physical interface for the organization in
        the \nWatson IoT Platform."
      operationId: creates-a-new-draft-physical-interface-for-the-organization-in-the-watson-iot-platform
      x-api-path-slug: draftphysicalinterfaces-post
      parameters:
      - in: body
        name: Physical Interface
        description: The JSON representation of the physical interface
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Physicalinterfaces
  /draft/physicalinterfaces/{physicalInterfaceId}:
    get:
      summary: Get a draft physical interface
      description: Retrieve the draft physical interface with the specified id.
      operationId: retrieve-the-draft-physical-interface-with-the-specified-id
      x-api-path-slug: draftphysicalinterfacesphysicalinterfaceid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Physicalinterfaces
      - PhysicalInterfaceId
    put:
      summary: Update a draft physical interface
      description: "Updates the draft physical interface with the specified id. The
        \nfollowing properties can be updated:\n\n  - name\n  - description\n\nNote
        that if the description field is omitted from the body of the\nupdate, then
        any existing description will be removed from the physical\ninterface.\n  \nAny
        changes made to the values of the following properties will be\nignored:\n\n
        \ - created\n  - createdBy\n  - updated\n  - updatedBy\n  - refs\n  \nThe
        values of these properties are set on the server as a result of a\nsuccessful
        update."
      operationId: updates-the-draft-physical-interface-with-the-specified-id-the-following-properties-can-be-updated--
      x-api-path-slug: draftphysicalinterfacesphysicalinterfaceid-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: Physical Interface
        description: The JSON representation of the physical interface
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Physicalinterfaces
      - PhysicalInterfaceId
    delete:
      summary: Delete a draft physical interface
      description: |-
        Deletes the draft physical interface with the specified id from the
        organization in the Watson IoT Platform.

        Please note the the delete will fail if the draft physical interface is
        being referenced  by a device type.
      operationId: deletes-the-draft-physical-interface-with-the-specified-id-from-theorganization-in-the-watson-iot-pl
      x-api-path-slug: draftphysicalinterfacesphysicalinterfaceid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Physicalinterfaces
      - PhysicalInterfaceId
  /draft/physicalinterfaces/{physicalInterfaceId}/events:
    get:
      summary: Get the list of event mappings
      description: |-
        Retrieve the list of event mappings for the draft physical interface.
        Event mappings are keyed off of the event id specified in the MQTT topic
        that the inbound events are published to.
      operationId: retrieve-the-list-of-event-mappings-for-the-draft-physical-interfaceevent-mappings-are-keyed-off-of-
      x-api-path-slug: draftphysicalinterfacesphysicalinterfaceidevents-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Physicalinterfaces
      - PhysicalInterfaceId
      - Events
    post:
      summary: Map an event to the draft physical interface
      description: |-
        Maps an event id to a specific event type for the draft specified
        physical interface.
      operationId: maps-an-event-id-to-a-specific-event-type-for-the-draft-specifiedphysical-interface
      x-api-path-slug: draftphysicalinterfacesphysicalinterfaceidevents-post
      parameters:
      - in: body
        name: Event Mapping
        description: The JSON representation of the event mapping
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Physicalinterfaces
      - PhysicalInterfaceId
      - Events
  /draft/physicalinterfaces/{physicalInterfaceId}/events/{eventId}:
    delete:
      summary: Remove an event mapping from the draft physical interface
      description: |-
        Removes the event mapping with the specified id from the draft physical
        interface.
      operationId: removes-the-event-mapping-with-the-specified-id-from-the-draft-physicalinterface
      x-api-path-slug: draftphysicalinterfacesphysicalinterfaceideventseventid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Physicalinterfaces
      - PhysicalInterfaceId
      - Events
      - EventId
  /logicalinterfaces:
    get:
      summary: Query active logical interfaces
      description: |-
        Logical interfaces are used to model the interfaces exposed by a
        device or thing in the Watson IoT Platform. A logical interface
        must reference a schema definition that defines the structure of the
        state that will be stored for the device or thing.

        The **logicalinterfaces** endpoint returns the list of all of the
        active logical interfaces that have been defined for the organization
        in the Watson IoT Platform.  Various query parameters can
        be used to filter, sort and page through the list of active logical
        interfaces that are returned.
      operationId: logical-interfaces-are-used-to-model-the-interfaces-exposed-by-adevice-or-thing-in-the-watson-iot-pl
      x-api-path-slug: logicalinterfaces-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Logical interfaces
  /logicalinterfaces/{logicalInterfaceId}:
    get:
      summary: Get an active logical interface
      description: Retrieve the active logical interface with the specified id.
      operationId: retrieve-the-active-logical-interface-with-the-specified-id
      x-api-path-slug: logicalinterfaceslogicalinterfaceid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Logical interfaces
      - LogicalInterfaceId
    patch:
      summary: Perform an operation against a logical interface
      description: |-
        Performs the specified operation against the logical interface. The
        following values can be specified for the operation property:

          - deactivate-configuration

        The **deactivate-configuration** operation will remove any active
        configuration that is currently associated with the logical
        interface. If the logical interface is associated with any device
        types, the state for any instances of those device types will be deleted
        as a result of performing the **deactivate-configuration** operation.
        The **deactivate-configuration** operation will fail if the logical
        interface is referenced by a thing schema.
      operationId: performs-the-specified-operation-against-the-logical-interface-thefollowing-values-can-be-specified-
      x-api-path-slug: logicalinterfaceslogicalinterfaceid-patch
      parameters:
      - in: query
        name: No Name
      - in: body
        name: Operation
        description: The JSON representation of an operation
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Logical interfaces
      - LogicalInterfaceId
  /draft/logicalinterfaces:
    get:
      summary: Query draft logical interfaces
      description: |-
        Logical interfaces are used to model the interfaces exposed by a
        device or thing in the Watson IoT Platform. A logical interface must
        reference a schema definition that defines the structure of the
        state that will be stored for the device or thing.

        The **logicalinterfaces** endpoint returns the list of all of the
        draft logical interfaces that have been defined for the organization
        in the Watson IoT Platform.  Various query parameters can be used to
        filter, sort and page through the list of draft logical interfaces
        that are returned.
      operationId: logical-interfaces-are-used-to-model-the-interfaces-exposed-by-adevice-or-thing-in-the-watson-iot-pl
      x-api-path-slug: draftlogicalinterfaces-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Logical interfaces
    post:
      summary: Create a draft logical interface
      description: |-
        Creates a new draft logical interface for the organization in the
        Watson IoT Platform. The logical interface must reference a schema
        definition that defines the structure of the state that will be stored
        for the device or thing.
      operationId: creates-a-new-draft-logical-interface-for-the-organization-in-thewatson-iot-platform-the-logical-int
      x-api-path-slug: draftlogicalinterfaces-post
      parameters:
      - in: body
        name: Logical Interface
        description: The JSON representation of the draft logical interface
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Logical interfaces
  /draft/logicalinterfaces/{logicalInterfaceId}:
    get:
      summary: Get a draft logical interface
      description: Retrieve the draft logical interface with the specified id.
      operationId: retrieve-the-draft-logical-interface-with-the-specified-id
      x-api-path-slug: draftlogicalinterfaceslogicalinterfaceid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Logical interfaces
      - LogicalInterfaceId
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