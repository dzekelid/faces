---
swagger: "2.0"
x-collection-name: IBM Watson
x-complete: 0
info:
  title: IBM Watson IoT Platform Query draft phyiscal interfaces
  description: "Physical interfaces are used to model the interfaces between physical\ndevices
    and the Watson IoT Platform.  A physical interface references\nevent types.  Devices
    that implement a physical interface publish these\nevents to the platform.\n\nThe
    event types are referenced via a mapping that maps an event id to\nthe id of an
    event type.  The event id corresponds to the MQTT topic\nthat the event is published
    to by a device.\n\nThe **/draft/physicalinterfaces** endpoint returns the list
    of all of \nthe draft physical interfaces that have been defined for the\norganization
    in the Watson IoT Platform.  Various query parameters can\nbe used to filter,
    sort and page through the list of draft physical\ninterfaces that are returned."
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