---
name: IBM Watson
x-slug: ibm-watson
description: Meet IBM Watson, a cognitive system that enables a new partnership between
  people and computers that enhances and scales human expertise. Watson has been learning
  the language of professions and is trained by experts to work across many different
  industries.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Faces
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/apis.md
specificationVersion: "0.14"
apis:
- name: IBM Watson IoT Platform Query active phyiscal interfaces
  x-api-slug: ibm-watson-iot-platform
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//physicalinterfaces
  tags: Internet of Things,Physicalinterfaces
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/physicalinterfaces-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/physicalinterfaces-get-openapi.md
- name: IBM Watson IoT Platform Get an active physical interface
  x-api-slug: ibm-watson-iot-platform
  description: Retrieve the active physical interface with the specified id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//physicalinterfaces/{physicalInterfaceId}
  tags: Internet of Things,Physicalinterfaces,PhysicalInterfaceId
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/physicalinterfacesphysicalinterfaceid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/physicalinterfacesphysicalinterfaceid-get-openapi.md
- name: IBM Watson IoT Platform Get the list of event mappings
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Retrieve the list of event mappings for the active physical interface.
    Event mappings are keyed off of the event id specified in the MQTT topic
    that the inbound events are published to.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//physicalinterfaces/{physicalInterfaceId}/events
  tags: Internet of Things,Physicalinterfaces,PhysicalInterfaceId,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/physicalinterfacesphysicalinterfaceidevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/physicalinterfacesphysicalinterfaceidevents-get-openapi.md
- name: IBM Watson IoT Platform Query draft phyiscal interfaces
  x-api-slug: ibm-watson-iot-platform
  description: "Physical interfaces are used to model the interfaces between physical\ndevices
    and the Watson IoT Platform.  A physical interface references\nevent types.  Devices
    that implement a physical interface publish these\nevents to the platform.\n\nThe
    event types are referenced via a mapping that maps an event id to\nthe id of an
    event type.  The event id corresponds to the MQTT topic\nthat the event is published
    to by a device.\n\nThe **/draft/physicalinterfaces** endpoint returns the list
    of all of \nthe draft physical interfaces that have been defined for the\norganization
    in the Watson IoT Platform.  Various query parameters can\nbe used to filter,
    sort and page through the list of draft physical\ninterfaces that are returned."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/physicalinterfaces
  tags: Internet of Things,Draft,Physicalinterfaces
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftphysicalinterfaces-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftphysicalinterfaces-get-openapi.md
- name: IBM Watson IoT Platform Create a draft physical interface
  x-api-slug: ibm-watson-iot-platform
  description: "Creates a new draft physical interface for the organization in the
    \nWatson IoT Platform."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/physicalinterfaces
  tags: Internet of Things,Draft,Physicalinterfaces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftphysicalinterfaces-post-openapi.md
- name: IBM Watson IoT Platform Get a draft physical interface
  x-api-slug: ibm-watson-iot-platform
  description: Retrieve the draft physical interface with the specified id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/physicalinterfaces/{physicalInterfaceId}
  tags: Internet of Things,Draft,Physicalinterfaces,PhysicalInterfaceId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftphysicalinterfacesphysicalinterfaceid-get-openapi.md
- name: IBM Watson IoT Platform Update a draft physical interface
  x-api-slug: ibm-watson-iot-platform
  description: "Updates the draft physical interface with the specified id. The \nfollowing
    properties can be updated:\n\n  - name\n  - description\n\nNote that if the description
    field is omitted from the body of the\nupdate, then any existing description will
    be removed from the physical\ninterface.\n  \nAny changes made to the values of
    the following properties will be\nignored:\n\n  - created\n  - createdBy\n  -
    updated\n  - updatedBy\n  - refs\n  \nThe values of these properties are set on
    the server as a result of a\nsuccessful update."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/physicalinterfaces/{physicalInterfaceId}
  tags: Internet of Things,Draft,Physicalinterfaces,PhysicalInterfaceId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftphysicalinterfacesphysicalinterfaceid-put-openapi.md
- name: IBM Watson IoT Platform Delete a draft physical interface
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Deletes the draft physical interface with the specified id from the
    organization in the Watson IoT Platform.

    Please note the the delete will fail if the draft physical interface is
    being referenced  by a device type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/physicalinterfaces/{physicalInterfaceId}
  tags: Internet of Things,Draft,Physicalinterfaces,PhysicalInterfaceId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftphysicalinterfacesphysicalinterfaceid-delete-openapi.md
- name: IBM Watson IoT Platform Get the list of event mappings
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Retrieve the list of event mappings for the draft physical interface.
    Event mappings are keyed off of the event id specified in the MQTT topic
    that the inbound events are published to.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/physicalinterfaces/{physicalInterfaceId}/events
  tags: Internet of Things,Draft,Physicalinterfaces,PhysicalInterfaceId,Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftphysicalinterfacesphysicalinterfaceidevents-get-openapi.md
- name: IBM Watson IoT Platform Map an event to the draft physical interface
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Maps an event id to a specific event type for the draft specified
    physical interface.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/physicalinterfaces/{physicalInterfaceId}/events
  tags: Internet of Things,Draft,Physicalinterfaces,PhysicalInterfaceId,Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftphysicalinterfacesphysicalinterfaceidevents-post-openapi.md
- name: IBM Watson IoT Platform Remove an event mapping from the draft physical interface
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Removes the event mapping with the specified id from the draft physical
    interface.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/physicalinterfaces/{physicalInterfaceId}/events/{eventId}
  tags: Internet of Things,Draft,Physicalinterfaces,PhysicalInterfaceId,Events,EventId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftphysicalinterfacesphysicalinterfaceideventseventid-delete-openapi.md
- name: IBM Watson IoT Platform Query active logical interfaces
  x-api-slug: ibm-watson-iot-platform
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//logicalinterfaces
  tags: Internet of Things,Logical interfaces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/logicalinterfaces-get-openapi.md
- name: IBM Watson IoT Platform Get an active logical interface
  x-api-slug: ibm-watson-iot-platform
  description: Retrieve the active logical interface with the specified id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//logicalinterfaces/{logicalInterfaceId}
  tags: Internet of Things,Logical interfaces,LogicalInterfaceId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/logicalinterfaceslogicalinterfaceid-get-openapi.md
- name: IBM Watson IoT Platform Perform an operation against a logical interface
  x-api-slug: ibm-watson-iot-platform
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//logicalinterfaces/{logicalInterfaceId}
  tags: Internet of Things,Logical interfaces,LogicalInterfaceId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/logicalinterfaceslogicalinterfaceid-patch-openapi.md
- name: IBM Watson IoT Platform Query draft logical interfaces
  x-api-slug: ibm-watson-iot-platform
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/logicalinterfaces
  tags: Internet of Things,Draft,Logical interfaces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftlogicalinterfaces-get-openapi.md
- name: IBM Watson IoT Platform Create a draft logical interface
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Creates a new draft logical interface for the organization in the
    Watson IoT Platform. The logical interface must reference a schema
    definition that defines the structure of the state that will be stored
    for the device or thing.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/logicalinterfaces
  tags: Internet of Things,Draft,Logical interfaces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftlogicalinterfaces-post-openapi.md
- name: IBM Watson IoT Platform Get a draft logical interface
  x-api-slug: ibm-watson-iot-platform
  description: Retrieve the draft logical interface with the specified id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/logicalinterfaces/{logicalInterfaceId}
  tags: Internet of Things,Draft,Logical interfaces,LogicalInterfaceId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftlogicalinterfaceslogicalinterfaceid-get-openapi.md
- name: IBM Watson IoT Platform Update a draft logical interface
  x-api-slug: ibm-watson-iot-platform
  description: "Updates the draft logical interface with the specified id. The\nfollowing
    properties can be updated: \n\n  - name\n  - description\n  - schemaId\n\nNote
    that if the description field is omitted from the body of the\nupdate, then any
    existing description will be removed from the logical\ninterface.\n  \nAny changes
    made to the values of the following properties will be\nignored:\n\n  - created\n
    \ - createdBy\n  - updated\n  - updatedBy\n  - refs\n  \nThe values of these properties
    are set on the server as a result of a\nsuccessful update."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/logicalinterfaces/{logicalInterfaceId}
  tags: Internet of Things,Draft,Logical interfaces,LogicalInterfaceId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftlogicalinterfaceslogicalinterfaceid-put-openapi.md
- name: IBM Watson IoT Platform Perform an operation against a draft logical interface
  x-api-slug: ibm-watson-iot-platform
  description: "Performs the specified operation against the draft logical\ninterface.
    The following values can be specified for the operation\nproperty:\n\n  - validate-configuration\n
    \ - activate-configuration\n  - list-differences\n\nThe **validate-configuration**
    operation will analyze all of the \nconfiguration associated with the draft logical
    interface to\ndetermine if it is valid.  If the configuration is invalid, a list
    of \nthe issues will be returned in the body of the response.  \n \nThe **activate-configuration**
    operation will make the configuration\nassociated with the draft logical interface
    active. The \n**activate-configuration** operation must have been performed against\na
    draft logical interface before any state is generated for device\nor thing types
    that are associated with that logical interface.\n\nThe **list-differences** operation
    will return a list of the differences\nthat exist between the active configuration
    for the logical\ninterface, if any, and the draft configuration."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/logicalinterfaces/{logicalInterfaceId}
  tags: Internet of Things,Draft,Logical interfaces,LogicalInterfaceId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftlogicalinterfaceslogicalinterfaceid-patch-openapi.md
- name: IBM Watson IoT Platform Delete a draft logical interface
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Deletes the draft logical interface with the specified id from the
    organization in the Watson IoT Platform.

    Please note the the delete will fail if the draft logical interface
    is being referenced by a device type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/logicalinterfaces/{logicalInterfaceId}
  tags: Internet of Things,Draft,Logical interfaces,LogicalInterfaceId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftlogicalinterfaceslogicalinterfaceid-delete-openapi.md
- name: IBM Watson IoT Platform Query active rules
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Rules allow you to specify conditions that can be used to trigger
    actions. For example, you might create a rule that sends an email if
    the temperature of a device exceeds a certain value.

    Rules are defined against a specific logical interface schema.  At
    runtime, a rule will be evaluated whenever the state for a Device that
    exposes the logical interface changes.

    The **/logicalinterfaces/{logicalInterfaceId}/rules** endpoint returns
    the list of all of the active rules that have been associated with the
    logical interface. Various query parameters can be used to filter, sort
    and page through the list of rules that are returned.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//logicalinterfaces/{logicalInterfaceId}/rules
  tags: Internet of Things,Logical interfaces,LogicalInterfaceId,Rules
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/logicalinterfaceslogicalinterfaceidrules-get-openapi.md
- name: IBM Watson IoT Platform Get an active rule
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Retrieve the active rule with the specified id that has been associated
    with the specified logical interface.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//logicalinterfaces/{logicalInterfaceId}/rules/{ruleId}
  tags: Internet of Things,Logical interfaces,LogicalInterfaceId,Rules,RuleId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/logicalinterfaceslogicalinterfaceidrulesruleid-get-openapi.md
- name: IBM Watson IoT Platform Query draft rules
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Rules allow you to specify conditions that can be used to trigger
    actions. For example, you might create a rule that sends an email if
    the temperature of a device exceeds a certain value.

    Rules are defined against a specific logical interface schema.  At
    runtime, a rule will be evaluated whenever the state for a Device that
    exposes the logical interface changes.

    The **/draft/logicalinterfaces/{logicalInterfaceId}/rules** endpoint
    returns the list of all of the draft rules that have been associated
    with the logical interface. Various query parameters can be used to
    filter, sort and page through the list of rules that are returned.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/logicalinterfaces/{logicalInterfaceId}/rules
  tags: Internet of Things,Draft,Logical interfaces,LogicalInterfaceId,Rules
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftlogicalinterfaceslogicalinterfaceidrules-get-openapi.md
- name: IBM Watson IoT Platform Create a draft rule
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Creates a new draft rule that is associated with the logical interface
    for the organization in the Watson IoT Platform.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/logicalinterfaces/{logicalInterfaceId}/rules
  tags: Internet of Things,Draft,Logical interfaces,LogicalInterfaceId,Rules
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftlogicalinterfaceslogicalinterfaceidrules-post-openapi.md
- name: IBM Watson IoT Platform Get a draft rule
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Retrieve the draft rule with the specified id that has been associated
    with the specified logical interface.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/logicalinterfaces/{logicalInterfaceId}/rules/{ruleId}
  tags: Internet of Things,Draft,Logical interfaces,LogicalInterfaceId,Rules,RuleId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftlogicalinterfaceslogicalinterfaceidrulesruleid-get-openapi.md
- name: IBM Watson IoT Platform Update a draft rule
  x-api-slug: ibm-watson-iot-platform
  description: "Updates the draft rule with the specified id. The following properties\ncan
    be updated: \n\n  - name\n  - description\n  - condition\n\nNote that if the description
    field is omitted from the body of the\nupdate, then any existing description will
    be removed from the rule.\n  \nAny changes made to the values of the following
    properties will be\nignored:\n\n  - created\n  - createdBy\n  - updated\n  - updatedBy\n
    \ - refs\n  \nThe values of these properties are set on the server as a result
    of a\nsuccessful update."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/logicalinterfaces/{logicalInterfaceId}/rules/{ruleId}
  tags: Internet of Things,Draft,Logical interfaces,LogicalInterfaceId,Rules,RuleId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftlogicalinterfaceslogicalinterfaceidrulesruleid-put-openapi.md
- name: IBM Watson IoT Platform Delete a draft rule
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Deletes the draft rule with the specified id from the organization in
    the Watson IoT Platform.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/logicalinterfaces/{logicalInterfaceId}/rules/{ruleId}
  tags: Internet of Things,Draft,Logical interfaces,LogicalInterfaceId,Rules,RuleId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftlogicalinterfaceslogicalinterfaceidrulesruleid-delete-openapi.md
- name: |-
    IBM Watson IoT Platform Get the list of active logical interfaces associated with the device
    type
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Retrieve the list of active logical interfaces that have been
    associated with the device type.  At least one logical interface
    must be associated with the device type before any mappings can be
    defined that will generate state for the device.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//device/types/{typeId}/logicalinterfaces
  tags: Internet of Things,Device,Types,Logical interfaces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/devicetypestypeidlogicalinterfaces-get-openapi.md
- name: |-
    IBM Watson IoT Platform Get the list of draft logical interfaces associated with the device
    type
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Retrieve the list of draft logical interfaces that have been
    associated with the device type.  At least one active logical
    interface must be associated with the device type before any mappings
    can be defined that will generate state for the device.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/device/types/{typeId}/logicalinterfaces
  tags: Internet of Things,Draft,Device,Types,Logical interfaces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftdevicetypestypeidlogicalinterfaces-get-openapi.md
- name: IBM Watson IoT Platform Associate a draft logical interface with the device
    type
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Associates a draft logical interface with the specified device type.
    The draft logical interface must already exist within the organization
    in the Watson IoT Platform.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/device/types/{typeId}/logicalinterfaces
  tags: Internet of Things,Draft,Device,Types,Logical interfaces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftdevicetypestypeidlogicalinterfaces-post-openapi.md
- name: IBM Watson IoT Platform Disassociate a draft logical interface from the device
    type
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Disassociates the draft logical interface  with the specified id
    from the device type.

    Please note the the delete will fail if the draft logical interface
    being removed from the device type is referenced in the property
    mappings for the device type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/device/types/{typeId}/logicalinterfaces/{logicalInterfaceId}
  tags: Internet of Things,Draft,Device,Types,Logical interfaces,LogicalInterfaceId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftdevicetypestypeidlogicalinterfaceslogicalinterfaceid-delete-openapi.md
- name: |-
    IBM Watson IoT Platform Get the list of active logical interfaces associated with the thing
    type
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Retrieve the list of active logical  interfaces that have been associated
    with the thing type.  At least one logical interface must be associated
    with the thing type before any mappings can be defined that will generate
    state for the thing.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//thing/types/{thingTypeId}/logicalinterfaces
  tags: Internet of Things,Thing,Types,ThingTypeId,Logical interfaces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/thingtypesthingtypeidlogicalinterfaces-get-openapi.md
- name: |-
    IBM Watson IoT Platform Get the list of draft logical interfaces associated with the thing
    type
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Retrieve the list of draft logical interfaces that have been associated
    with the draft thing type.  At least one logical interface must be
    associated with the thing type before any mappings can be defined that
    will generate state for the thing.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/thing/types/{thingTypeId}/logicalinterfaces
  tags: Internet of Things,Draft,Thing,Types,ThingTypeId,Logical interfaces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftthingtypesthingtypeidlogicalinterfaces-get-openapi.md
- name: IBM Watson IoT Platform Associate a draft logical interface with the draft
    thing type
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Associates a draft logical interface with the specified draft thing type.
    The logical interface must already exist within the organization in the
    Watson IoT Platform.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/thing/types/{thingTypeId}/logicalinterfaces
  tags: Internet of Things,Draft,Thing,Types,ThingTypeId,Logical interfaces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftthingtypesthingtypeidlogicalinterfaces-post-openapi.md
- name: IBM Watson IoT Platform Disassociate a logical interface from the draft thing
    type
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Disassociates the draft logical interface with the specified id from the
    draft thing type.

    Please note the the delete will fail if the logical interface being
    removed from the draft thing type is referenced in the property mappings
    for the draft thing type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/thing/types/{thingTypeId}/logicalinterfaces/{logicalInterfaceId}
  tags: Internet of Things,Draft,Thing,Types,ThingTypeId,Logical interfaces,LogicalInterfaceId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/draftthingtypesthingtypeidlogicalinterfaceslogicalinterfaceid-delete-openapi.md
- name: IBM Watson IoT Platform
  x-api-slug: ibm-watson-iot-platform
  description: Meet IBM Watson, a cognitive system that enables a new partnership
    between people and computers that enhances and scales human expertise. Watson
    has been learning the language of professions and is trained by experts to work
    across many different industries.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002
  tags: Faces
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/faces/master/_listings/ibm-watson/openapi.md
x-common:
- type: x-application-gallery
  url: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/gallery.html
- type: x-blog
  url: https://developer.ibm.com/watson/blog/
- type: x-blog-rss
  url: https://developer.ibm.com/watson/feed/
- type: x-developer
  url: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/doc/
- type: x-developer
  url: https://developer.ibm.com/watson/
- type: x-documentation
  url: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/apis/
- type: x-forum
  url: https://developer.ibm.com/answers/smartspace/watson/
- type: x-getting-started
  url: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/getstarted.html
- type: x-github
  url: https://github.com/IBM-Watson
- type: x-partners
  url: http://www.ibm.com/smarterplanet/us/en/ibmwatson/ecosystem.html
- type: x-privacy
  url: http://www.ibm.com/privacy/us/en/?lnk=flg-priv-usen
- type: x-terms-of-service
  url: http://www.ibm.com/legal/us/en/?lnk=flg-tous-usen
- type: x-twitter
  url: https://twitter.com/IBMWatson
- type: x-videos
  url: http://www.ibm.com/smarterplanet/us/en/ibmwatson/
- type: x-website
  url: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
- type: x-white-papers
  url: https://developer.ibm.com/watson/docs/whitepapers/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---