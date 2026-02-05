---
permalink: /upbound-provider-azuread/cluster/groups/v1beta2/group/
---

# groups.v1beta2.group

"Group is the Schema for the Groups API."

## Index

* [`fn new(name)`](#fn-new)
* [`obj metadata`](#obj-metadata)
  * [`fn withAnnotations(annotations)`](#fn-metadatawithannotations)
  * [`fn withAnnotationsMixin(annotations)`](#fn-metadatawithannotationsmixin)
  * [`fn withClusterName(clusterName)`](#fn-metadatawithclustername)
  * [`fn withCreationTimestamp(creationTimestamp)`](#fn-metadatawithcreationtimestamp)
  * [`fn withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)`](#fn-metadatawithdeletiongraceperiodseconds)
  * [`fn withDeletionTimestamp(deletionTimestamp)`](#fn-metadatawithdeletiontimestamp)
  * [`fn withFinalizers(finalizers)`](#fn-metadatawithfinalizers)
  * [`fn withFinalizersMixin(finalizers)`](#fn-metadatawithfinalizersmixin)
  * [`fn withGenerateName(generateName)`](#fn-metadatawithgeneratename)
  * [`fn withGeneration(generation)`](#fn-metadatawithgeneration)
  * [`fn withLabels(labels)`](#fn-metadatawithlabels)
  * [`fn withLabelsMixin(labels)`](#fn-metadatawithlabelsmixin)
  * [`fn withName(name)`](#fn-metadatawithname)
  * [`fn withNamespace(namespace)`](#fn-metadatawithnamespace)
  * [`fn withOwnerReferences(ownerReferences)`](#fn-metadatawithownerreferences)
  * [`fn withOwnerReferencesMixin(ownerReferences)`](#fn-metadatawithownerreferencesmixin)
  * [`fn withResourceVersion(resourceVersion)`](#fn-metadatawithresourceversion)
  * [`fn withSelfLink(selfLink)`](#fn-metadatawithselflink)
  * [`fn withUid(uid)`](#fn-metadatawithuid)
* [`obj spec`](#obj-spec)
  * [`fn withDeletionPolicy(deletionPolicy)`](#fn-specwithdeletionpolicy)
  * [`fn withManagementPolicies(managementPolicies)`](#fn-specwithmanagementpolicies)
  * [`fn withManagementPoliciesMixin(managementPolicies)`](#fn-specwithmanagementpoliciesmixin)
  * [`obj spec.forProvider`](#obj-specforprovider)
    * [`fn withAdministrativeUnitIds(administrativeUnitIds)`](#fn-specforproviderwithadministrativeunitids)
    * [`fn withAdministrativeUnitIdsMixin(administrativeUnitIds)`](#fn-specforproviderwithadministrativeunitidsmixin)
    * [`fn withAssignableToRole(assignableToRole)`](#fn-specforproviderwithassignabletorole)
    * [`fn withAutoSubscribeNewMembers(autoSubscribeNewMembers)`](#fn-specforproviderwithautosubscribenewmembers)
    * [`fn withBehaviors(behaviors)`](#fn-specforproviderwithbehaviors)
    * [`fn withBehaviorsMixin(behaviors)`](#fn-specforproviderwithbehaviorsmixin)
    * [`fn withDescription(description)`](#fn-specforproviderwithdescription)
    * [`fn withDisplayName(displayName)`](#fn-specforproviderwithdisplayname)
    * [`fn withExternalSendersAllowed(externalSendersAllowed)`](#fn-specforproviderwithexternalsendersallowed)
    * [`fn withHideFromAddressLists(hideFromAddressLists)`](#fn-specforproviderwithhidefromaddresslists)
    * [`fn withHideFromOutlookClients(hideFromOutlookClients)`](#fn-specforproviderwithhidefromoutlookclients)
    * [`fn withMailEnabled(mailEnabled)`](#fn-specforproviderwithmailenabled)
    * [`fn withMailNickname(mailNickname)`](#fn-specforproviderwithmailnickname)
    * [`fn withMembers(members)`](#fn-specforproviderwithmembers)
    * [`fn withMembersMixin(members)`](#fn-specforproviderwithmembersmixin)
    * [`fn withMembersRefs(membersRefs)`](#fn-specforproviderwithmembersrefs)
    * [`fn withMembersRefsMixin(membersRefs)`](#fn-specforproviderwithmembersrefsmixin)
    * [`fn withOnpremisesGroupType(onpremisesGroupType)`](#fn-specforproviderwithonpremisesgrouptype)
    * [`fn withOwners(owners)`](#fn-specforproviderwithowners)
    * [`fn withOwnersMixin(owners)`](#fn-specforproviderwithownersmixin)
    * [`fn withPreventDuplicateNames(preventDuplicateNames)`](#fn-specforproviderwithpreventduplicatenames)
    * [`fn withProvisioningOptions(provisioningOptions)`](#fn-specforproviderwithprovisioningoptions)
    * [`fn withProvisioningOptionsMixin(provisioningOptions)`](#fn-specforproviderwithprovisioningoptionsmixin)
    * [`fn withSecurityEnabled(securityEnabled)`](#fn-specforproviderwithsecurityenabled)
    * [`fn withTheme(theme)`](#fn-specforproviderwiththeme)
    * [`fn withTypes(types)`](#fn-specforproviderwithtypes)
    * [`fn withTypesMixin(types)`](#fn-specforproviderwithtypesmixin)
    * [`fn withVisibility(visibility)`](#fn-specforproviderwithvisibility)
    * [`fn withWritebackEnabled(writebackEnabled)`](#fn-specforproviderwithwritebackenabled)
    * [`obj spec.forProvider.dynamicMembership`](#obj-specforproviderdynamicmembership)
      * [`fn withEnabled(enabled)`](#fn-specforproviderdynamicmembershipwithenabled)
      * [`fn withRule(rule)`](#fn-specforproviderdynamicmembershipwithrule)
    * [`obj spec.forProvider.membersRefs`](#obj-specforprovidermembersrefs)
      * [`fn withName(name)`](#fn-specforprovidermembersrefswithname)
      * [`obj spec.forProvider.membersRefs.policy`](#obj-specforprovidermembersrefspolicy)
        * [`fn withResolution(resolution)`](#fn-specforprovidermembersrefspolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specforprovidermembersrefspolicywithresolve)
    * [`obj spec.forProvider.membersSelector`](#obj-specforprovidermembersselector)
      * [`fn withMatchControllerRef(matchControllerRef)`](#fn-specforprovidermembersselectorwithmatchcontrollerref)
      * [`fn withMatchLabels(matchLabels)`](#fn-specforprovidermembersselectorwithmatchlabels)
      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specforprovidermembersselectorwithmatchlabelsmixin)
      * [`obj spec.forProvider.membersSelector.policy`](#obj-specforprovidermembersselectorpolicy)
        * [`fn withResolution(resolution)`](#fn-specforprovidermembersselectorpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specforprovidermembersselectorpolicywithresolve)
  * [`obj spec.initProvider`](#obj-specinitprovider)
    * [`fn withAdministrativeUnitIds(administrativeUnitIds)`](#fn-specinitproviderwithadministrativeunitids)
    * [`fn withAdministrativeUnitIdsMixin(administrativeUnitIds)`](#fn-specinitproviderwithadministrativeunitidsmixin)
    * [`fn withAssignableToRole(assignableToRole)`](#fn-specinitproviderwithassignabletorole)
    * [`fn withAutoSubscribeNewMembers(autoSubscribeNewMembers)`](#fn-specinitproviderwithautosubscribenewmembers)
    * [`fn withBehaviors(behaviors)`](#fn-specinitproviderwithbehaviors)
    * [`fn withBehaviorsMixin(behaviors)`](#fn-specinitproviderwithbehaviorsmixin)
    * [`fn withDescription(description)`](#fn-specinitproviderwithdescription)
    * [`fn withDisplayName(displayName)`](#fn-specinitproviderwithdisplayname)
    * [`fn withExternalSendersAllowed(externalSendersAllowed)`](#fn-specinitproviderwithexternalsendersallowed)
    * [`fn withHideFromAddressLists(hideFromAddressLists)`](#fn-specinitproviderwithhidefromaddresslists)
    * [`fn withHideFromOutlookClients(hideFromOutlookClients)`](#fn-specinitproviderwithhidefromoutlookclients)
    * [`fn withMailEnabled(mailEnabled)`](#fn-specinitproviderwithmailenabled)
    * [`fn withMailNickname(mailNickname)`](#fn-specinitproviderwithmailnickname)
    * [`fn withMembers(members)`](#fn-specinitproviderwithmembers)
    * [`fn withMembersMixin(members)`](#fn-specinitproviderwithmembersmixin)
    * [`fn withMembersRefs(membersRefs)`](#fn-specinitproviderwithmembersrefs)
    * [`fn withMembersRefsMixin(membersRefs)`](#fn-specinitproviderwithmembersrefsmixin)
    * [`fn withOnpremisesGroupType(onpremisesGroupType)`](#fn-specinitproviderwithonpremisesgrouptype)
    * [`fn withOwners(owners)`](#fn-specinitproviderwithowners)
    * [`fn withOwnersMixin(owners)`](#fn-specinitproviderwithownersmixin)
    * [`fn withPreventDuplicateNames(preventDuplicateNames)`](#fn-specinitproviderwithpreventduplicatenames)
    * [`fn withProvisioningOptions(provisioningOptions)`](#fn-specinitproviderwithprovisioningoptions)
    * [`fn withProvisioningOptionsMixin(provisioningOptions)`](#fn-specinitproviderwithprovisioningoptionsmixin)
    * [`fn withSecurityEnabled(securityEnabled)`](#fn-specinitproviderwithsecurityenabled)
    * [`fn withTheme(theme)`](#fn-specinitproviderwiththeme)
    * [`fn withTypes(types)`](#fn-specinitproviderwithtypes)
    * [`fn withTypesMixin(types)`](#fn-specinitproviderwithtypesmixin)
    * [`fn withVisibility(visibility)`](#fn-specinitproviderwithvisibility)
    * [`fn withWritebackEnabled(writebackEnabled)`](#fn-specinitproviderwithwritebackenabled)
    * [`obj spec.initProvider.dynamicMembership`](#obj-specinitproviderdynamicmembership)
      * [`fn withEnabled(enabled)`](#fn-specinitproviderdynamicmembershipwithenabled)
      * [`fn withRule(rule)`](#fn-specinitproviderdynamicmembershipwithrule)
    * [`obj spec.initProvider.membersRefs`](#obj-specinitprovidermembersrefs)
      * [`fn withName(name)`](#fn-specinitprovidermembersrefswithname)
      * [`obj spec.initProvider.membersRefs.policy`](#obj-specinitprovidermembersrefspolicy)
        * [`fn withResolution(resolution)`](#fn-specinitprovidermembersrefspolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specinitprovidermembersrefspolicywithresolve)
    * [`obj spec.initProvider.membersSelector`](#obj-specinitprovidermembersselector)
      * [`fn withMatchControllerRef(matchControllerRef)`](#fn-specinitprovidermembersselectorwithmatchcontrollerref)
      * [`fn withMatchLabels(matchLabels)`](#fn-specinitprovidermembersselectorwithmatchlabels)
      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specinitprovidermembersselectorwithmatchlabelsmixin)
      * [`obj spec.initProvider.membersSelector.policy`](#obj-specinitprovidermembersselectorpolicy)
        * [`fn withResolution(resolution)`](#fn-specinitprovidermembersselectorpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specinitprovidermembersselectorpolicywithresolve)
  * [`obj spec.providerConfigRef`](#obj-specproviderconfigref)
    * [`fn withName(name)`](#fn-specproviderconfigrefwithname)
    * [`obj spec.providerConfigRef.policy`](#obj-specproviderconfigrefpolicy)
      * [`fn withResolution(resolution)`](#fn-specproviderconfigrefpolicywithresolution)
      * [`fn withResolve(resolve)`](#fn-specproviderconfigrefpolicywithresolve)
  * [`obj spec.writeConnectionSecretToRef`](#obj-specwriteconnectionsecrettoref)
    * [`fn withName(name)`](#fn-specwriteconnectionsecrettorefwithname)
    * [`fn withNamespace(namespace)`](#fn-specwriteconnectionsecrettorefwithnamespace)

## Fields

### fn new

```ts
new(name)
```

new returns an instance of Group

## obj metadata

"ObjectMeta is metadata that all persisted resources must have, which includes all objects users must create."

### fn metadata.withAnnotations

```ts
withAnnotations(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

### fn metadata.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

**Note:** This function appends passed data to existing values

### fn metadata.withClusterName

```ts
withClusterName(clusterName)
```

"The name of the cluster which the object belongs to. This is used to distinguish resources with same name and namespace in different clusters. This field is not set anywhere right now and apiserver is going to ignore it if set in create or update request."

### fn metadata.withCreationTimestamp

```ts
withCreationTimestamp(creationTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withDeletionGracePeriodSeconds

```ts
withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)
```

"Number of seconds allowed for this object to gracefully terminate before it will be removed from the system. Only set when deletionTimestamp is also set. May only be shortened. Read-only."

### fn metadata.withDeletionTimestamp

```ts
withDeletionTimestamp(deletionTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withFinalizers

```ts
withFinalizers(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

### fn metadata.withFinalizersMixin

```ts
withFinalizersMixin(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

**Note:** This function appends passed data to existing values

### fn metadata.withGenerateName

```ts
withGenerateName(generateName)
```

"GenerateName is an optional prefix, used by the server, to generate a unique name ONLY IF the Name field has not been provided. If this field is used, the name returned to the client will be different than the name passed. This value will also be combined with a unique suffix. The provided value has the same validation rules as the Name field, and may be truncated by the length of the suffix required to make the value unique on the server.\n\nIf this field is specified and the generated name exists, the server will NOT return a 409 - instead, it will either return 201 Created or 500 with Reason ServerTimeout indicating a unique name could not be found in the time allotted, and the client should retry (optionally after the time indicated in the Retry-After header).\n\nApplied only if Name is not specified. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#idempotency"

### fn metadata.withGeneration

```ts
withGeneration(generation)
```

"A sequence number representing a specific generation of the desired state. Populated by the system. Read-only."

### fn metadata.withLabels

```ts
withLabels(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

### fn metadata.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

**Note:** This function appends passed data to existing values

### fn metadata.withName

```ts
withName(name)
```

"Name must be unique within a namespace. Is required when creating resources, although some resources may allow a client to request the generation of an appropriate name automatically. Name is primarily intended for creation idempotence and configuration definition. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/identifiers#names"

### fn metadata.withNamespace

```ts
withNamespace(namespace)
```

"Namespace defines the space within which each name must be unique. An empty namespace is equivalent to the \"default\" namespace, but \"default\" is the canonical representation. Not all objects are required to be scoped to a namespace - the value of this field for those objects will be empty.\n\nMust be a DNS_LABEL. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/namespaces"

### fn metadata.withOwnerReferences

```ts
withOwnerReferences(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

### fn metadata.withOwnerReferencesMixin

```ts
withOwnerReferencesMixin(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

**Note:** This function appends passed data to existing values

### fn metadata.withResourceVersion

```ts
withResourceVersion(resourceVersion)
```

"An opaque value that represents the internal version of this object that can be used by clients to determine when objects have changed. May be used for optimistic concurrency, change detection, and the watch operation on a resource or set of resources. Clients must treat these values as opaque and passed unmodified back to the server. They may only be valid for a particular resource or set of resources.\n\nPopulated by the system. Read-only. Value must be treated as opaque by clients and . More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency"

### fn metadata.withSelfLink

```ts
withSelfLink(selfLink)
```

"SelfLink is a URL representing this object. Populated by the system. Read-only.\n\nDEPRECATED Kubernetes will stop propagating this field in 1.20 release and the field is planned to be removed in 1.21 release."

### fn metadata.withUid

```ts
withUid(uid)
```

"UID is the unique in time and space value for this object. It is typically generated by the server on successful creation of a resource and is not allowed to change on PUT operations.\n\nPopulated by the system. Read-only. More info: http://kubernetes.io/docs/user-guide/identifiers#uids"

## obj spec

"GroupSpec defines the desired state of Group"

### fn spec.withDeletionPolicy

```ts
withDeletionPolicy(deletionPolicy)
```

"DeletionPolicy specifies what will happen to the underlying external\nwhen this managed resource is deleted - either \"Delete\" or \"Orphan\" the\nexternal resource.\nThis field is planned to be deprecated in favor of the ManagementPolicies\nfield in a future release. Currently, both could be set independently and\nnon-default values would be honored if the feature flag is enabled.\nSee the design doc for more information: https://github.com/crossplane/crossplane/blob/499895a25d1a1a0ba1604944ef98ac7a1a71f197/design/design-doc-observe-only-resources.md?plain=1#L223"

### fn spec.withManagementPolicies

```ts
withManagementPolicies(managementPolicies)
```

"THIS IS A BETA FIELD. It is on by default but can be opted out\nthrough a Crossplane feature flag.\nManagementPolicies specify the array of actions Crossplane is allowed to\ntake on the managed and external resources.\nThis field is planned to replace the DeletionPolicy field in a future\nrelease. Currently, both could be set independently and non-default\nvalues would be honored if the feature flag is enabled. If both are\ncustom, the DeletionPolicy field will be ignored.\nSee the design doc for more information: https://github.com/crossplane/crossplane/blob/499895a25d1a1a0ba1604944ef98ac7a1a71f197/design/design-doc-observe-only-resources.md?plain=1#L223\nand this one: https://github.com/crossplane/crossplane/blob/444267e84783136daa93568b364a5f01228cacbe/design/one-pager-ignore-changes.md"

### fn spec.withManagementPoliciesMixin

```ts
withManagementPoliciesMixin(managementPolicies)
```

"THIS IS A BETA FIELD. It is on by default but can be opted out\nthrough a Crossplane feature flag.\nManagementPolicies specify the array of actions Crossplane is allowed to\ntake on the managed and external resources.\nThis field is planned to replace the DeletionPolicy field in a future\nrelease. Currently, both could be set independently and non-default\nvalues would be honored if the feature flag is enabled. If both are\ncustom, the DeletionPolicy field will be ignored.\nSee the design doc for more information: https://github.com/crossplane/crossplane/blob/499895a25d1a1a0ba1604944ef98ac7a1a71f197/design/design-doc-observe-only-resources.md?plain=1#L223\nand this one: https://github.com/crossplane/crossplane/blob/444267e84783136daa93568b364a5f01228cacbe/design/one-pager-ignore-changes.md"

**Note:** This function appends passed data to existing values

## obj spec.forProvider



### fn spec.forProvider.withAdministrativeUnitIds

```ts
withAdministrativeUnitIds(administrativeUnitIds)
```

"The object IDs of administrative units in which the group is a member. If specified, new groups will be created in the scope of the first administrative unit and added to the others. If empty, new groups will be created at the tenant level.\nThe administrative unit IDs in which the group should be. If empty, the group will be created at the tenant level."

### fn spec.forProvider.withAdministrativeUnitIdsMixin

```ts
withAdministrativeUnitIdsMixin(administrativeUnitIds)
```

"The object IDs of administrative units in which the group is a member. If specified, new groups will be created in the scope of the first administrative unit and added to the others. If empty, new groups will be created at the tenant level.\nThe administrative unit IDs in which the group should be. If empty, the group will be created at the tenant level."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withAssignableToRole

```ts
withAssignableToRole(assignableToRole)
```

"Indicates whether this group can be assigned to an Azure Active Directory role. Defaults to false. Can only be set to true for security-enabled groups. Changing this forces a new resource to be created.\nIndicates whether this group can be assigned to an Azure Active Directory role. This property can only be `true` for security-enabled groups."

### fn spec.forProvider.withAutoSubscribeNewMembers

```ts
withAutoSubscribeNewMembers(autoSubscribeNewMembers)
```

"Indicates whether new members added to the group will be auto-subscribed to receive email notifications. Can only be set for Unified groups.\nIndicates whether new members added to the group will be auto-subscribed to receive email notifications."

### fn spec.forProvider.withBehaviors

```ts
withBehaviors(behaviors)
```

"A set of behaviors for a Microsoft 365 group. Possible values are AllowOnlyMembersToPost, HideGroupInOutlook, SkipExchangeInstantOn, SubscribeMembersToCalendarEventsDisabled, SubscribeNewGroupMembers and WelcomeEmailDisabled. See official documentation for more details. Changing this forces a new resource to be created.\nThe group behaviours for a Microsoft 365 group"

### fn spec.forProvider.withBehaviorsMixin

```ts
withBehaviorsMixin(behaviors)
```

"A set of behaviors for a Microsoft 365 group. Possible values are AllowOnlyMembersToPost, HideGroupInOutlook, SkipExchangeInstantOn, SubscribeMembersToCalendarEventsDisabled, SubscribeNewGroupMembers and WelcomeEmailDisabled. See official documentation for more details. Changing this forces a new resource to be created.\nThe group behaviours for a Microsoft 365 group"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withDescription

```ts
withDescription(description)
```

"The description for the group.\nThe description for the group"

### fn spec.forProvider.withDisplayName

```ts
withDisplayName(displayName)
```

"The display name for the group.\nThe display name for the group"

### fn spec.forProvider.withExternalSendersAllowed

```ts
withExternalSendersAllowed(externalSendersAllowed)
```

"Indicates whether people external to the organization can send messages to the group. Can only be set for Unified groups.\nIndicates whether people external to the organization can send messages to the group."

### fn spec.forProvider.withHideFromAddressLists

```ts
withHideFromAddressLists(hideFromAddressLists)
```

"Indicates whether the group is displayed in certain parts of the Outlook user interface: in the Address Book, in address lists for selecting message recipients, and in the Browse Groups dialog for searching groups. Can only be set for Unified groups.\nIndicates whether the group is displayed in certain parts of the Outlook user interface: in the Address Book, in address lists for selecting message recipients, and in the Browse Groups dialog for searching groups."

### fn spec.forProvider.withHideFromOutlookClients

```ts
withHideFromOutlookClients(hideFromOutlookClients)
```

"Indicates whether the group is displayed in Outlook clients, such as Outlook for Windows and Outlook on the web. Can only be set for Unified groups.\nIndicates whether the group is displayed in Outlook clients, such as Outlook for Windows and Outlook on the web."

### fn spec.forProvider.withMailEnabled

```ts
withMailEnabled(mailEnabled)
```

"Whether the group is a mail enabled, with a shared group mailbox. At least one of mail_enabled or security_enabled must be specified. Only Microsoft 365 groups can be mail enabled (see the types property).\nWhether the group is a mail enabled, with a shared group mailbox. At least one of `mail_enabled` or `security_enabled` must be specified. A group can be mail enabled _and_ security enabled"

### fn spec.forProvider.withMailNickname

```ts
withMailNickname(mailNickname)
```

"The mail alias for the group, unique in the organisation. Required for mail-enabled groups. Changing this forces a new resource to be created.\nThe mail alias for the group, unique in the organisation"

### fn spec.forProvider.withMembers

```ts
withMembers(members)
```

"A set of members who should be present in this group. Supported object types are Users, Groups or Service Principals. Cannot be used with the dynamic_membership block.\nA set of members who should be present in this group. Supported object types are Users, Groups or Service Principals"

### fn spec.forProvider.withMembersMixin

```ts
withMembersMixin(members)
```

"A set of members who should be present in this group. Supported object types are Users, Groups or Service Principals. Cannot be used with the dynamic_membership block.\nA set of members who should be present in this group. Supported object types are Users, Groups or Service Principals"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withMembersRefs

```ts
withMembersRefs(membersRefs)
```

"References to User in users to populate members."

### fn spec.forProvider.withMembersRefsMixin

```ts
withMembersRefsMixin(membersRefs)
```

"References to User in users to populate members."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withOnpremisesGroupType

```ts
withOnpremisesGroupType(onpremisesGroupType)
```

"The on-premises group type that the AAD group will be written as, when writeback is enabled. Possible values are UniversalDistributionGroup, UniversalMailEnabledSecurityGroup, or UniversalSecurityGroup.\nIndicates the target on-premise group type the group will be written back as"

### fn spec.forProvider.withOwners

```ts
withOwners(owners)
```

"A set of object IDs of principals that will be granted ownership of the group. Supported object types are users or service principals. Groups cannot be created with no owners or have all their owners removed.\nA set of owners who own this group. Supported object types are Users or Service Principals"

### fn spec.forProvider.withOwnersMixin

```ts
withOwnersMixin(owners)
```

"A set of object IDs of principals that will be granted ownership of the group. Supported object types are users or service principals. Groups cannot be created with no owners or have all their owners removed.\nA set of owners who own this group. Supported object types are Users or Service Principals"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withPreventDuplicateNames

```ts
withPreventDuplicateNames(preventDuplicateNames)
```

"If true, will return an error if an existing group is found with the same name. Defaults to false.\nIf `true`, will return an error if an existing group is found with the same name"

### fn spec.forProvider.withProvisioningOptions

```ts
withProvisioningOptions(provisioningOptions)
```

"A set of provisioning options for a Microsoft 365 group. The only supported value is Team. See official documentation for details. Changing this forces a new resource to be created.\nThe group provisioning options for a Microsoft 365 group"

### fn spec.forProvider.withProvisioningOptionsMixin

```ts
withProvisioningOptionsMixin(provisioningOptions)
```

"A set of provisioning options for a Microsoft 365 group. The only supported value is Team. See official documentation for details. Changing this forces a new resource to be created.\nThe group provisioning options for a Microsoft 365 group"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withSecurityEnabled

```ts
withSecurityEnabled(securityEnabled)
```

"Whether the group is a security group for controlling access to in-app resources. At least one of security_enabled or mail_enabled must be specified. A Microsoft 365 group can be security enabled and mail enabled (see the types property).\nWhether the group is a security group for controlling access to in-app resources. At least one of `security_enabled` or `mail_enabled` must be specified. A group can be security enabled _and_ mail enabled"

### fn spec.forProvider.withTheme

```ts
withTheme(theme)
```

"The colour theme for a Microsoft 365 group. Possible values are Blue, Green, Orange, Pink, Purple, Red or Teal. By default, no theme is set.\nThe colour theme for a Microsoft 365 group"

### fn spec.forProvider.withTypes

```ts
withTypes(types)
```

"A set of group types to configure for the group. Supported values are DynamicMembership, which denotes a group with dynamic membership, and Unified, which specifies a Microsoft 365 group. Required when mail_enabled is true. Changing this forces a new resource to be created.\nA set of group types to configure for the group. `Unified` specifies a Microsoft 365 group. Required when `mail_enabled` is true"

### fn spec.forProvider.withTypesMixin

```ts
withTypesMixin(types)
```

"A set of group types to configure for the group. Supported values are DynamicMembership, which denotes a group with dynamic membership, and Unified, which specifies a Microsoft 365 group. Required when mail_enabled is true. Changing this forces a new resource to be created.\nA set of group types to configure for the group. `Unified` specifies a Microsoft 365 group. Required when `mail_enabled` is true"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withVisibility

```ts
withVisibility(visibility)
```

"The group join policy and group content visibility. Possible values are Private, Public, or Hiddenmembership. Only Microsoft 365 groups can have Hiddenmembership visibility and this value must be set when the group is created. By default, security groups will receive Private visibility and Microsoft 365 groups will receive Public visibility.\nSpecifies the group join policy and group content visibility"

### fn spec.forProvider.withWritebackEnabled

```ts
withWritebackEnabled(writebackEnabled)
```

"Whether the group will be written back to the configured on-premises Active Directory when Azure AD Connect is used.\nWhether this group should be synced from Azure AD to the on-premises directory when Azure AD Connect is used"

## obj spec.forProvider.dynamicMembership

"A dynamic_membership block as documented below. Required when types contains DynamicMembership. Cannot be used with the members property.\nAn optional block to configure dynamic membership for the group. Cannot be used with `members`"

### fn spec.forProvider.dynamicMembership.withEnabled

```ts
withEnabled(enabled)
```

"Whether rule processing is \"On\" (true) or \"Paused\" (false)."

### fn spec.forProvider.dynamicMembership.withRule

```ts
withRule(rule)
```

"The rule that determines membership of this group. For more information, see official documentation on membership rules syntax.\nRule to determine members for a dynamic group. Required when `group_types` contains 'DynamicMembership'"

## obj spec.forProvider.membersRefs

"References to User in users to populate members."

### fn spec.forProvider.membersRefs.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.forProvider.membersRefs.policy

"Policies for referencing."

### fn spec.forProvider.membersRefs.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.forProvider.membersRefs.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.forProvider.membersSelector

"Selector for a list of User in users to populate members."

### fn spec.forProvider.membersSelector.withMatchControllerRef

```ts
withMatchControllerRef(matchControllerRef)
```

"MatchControllerRef ensures an object with the same controller reference\nas the selecting object is selected."

### fn spec.forProvider.membersSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

### fn spec.forProvider.membersSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.membersSelector.policy

"Policies for selection."

### fn spec.forProvider.membersSelector.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.forProvider.membersSelector.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.initProvider

"THIS IS A BETA FIELD. It will be honored\nunless the Management Policies feature flag is disabled.\nInitProvider holds the same fields as ForProvider, with the exception\nof Identifier and other resource reference fields. The fields that are\nin InitProvider are merged into ForProvider when the resource is created.\nThe same fields are also added to the terraform ignore_changes hook, to\navoid updating them after creation. This is useful for fields that are\nrequired on creation, but we do not desire to update them after creation,\nfor example because of an external controller is managing them, like an\nautoscaler."

### fn spec.initProvider.withAdministrativeUnitIds

```ts
withAdministrativeUnitIds(administrativeUnitIds)
```

"The object IDs of administrative units in which the group is a member. If specified, new groups will be created in the scope of the first administrative unit and added to the others. If empty, new groups will be created at the tenant level.\nThe administrative unit IDs in which the group should be. If empty, the group will be created at the tenant level."

### fn spec.initProvider.withAdministrativeUnitIdsMixin

```ts
withAdministrativeUnitIdsMixin(administrativeUnitIds)
```

"The object IDs of administrative units in which the group is a member. If specified, new groups will be created in the scope of the first administrative unit and added to the others. If empty, new groups will be created at the tenant level.\nThe administrative unit IDs in which the group should be. If empty, the group will be created at the tenant level."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withAssignableToRole

```ts
withAssignableToRole(assignableToRole)
```

"Indicates whether this group can be assigned to an Azure Active Directory role. Defaults to false. Can only be set to true for security-enabled groups. Changing this forces a new resource to be created.\nIndicates whether this group can be assigned to an Azure Active Directory role. This property can only be `true` for security-enabled groups."

### fn spec.initProvider.withAutoSubscribeNewMembers

```ts
withAutoSubscribeNewMembers(autoSubscribeNewMembers)
```

"Indicates whether new members added to the group will be auto-subscribed to receive email notifications. Can only be set for Unified groups.\nIndicates whether new members added to the group will be auto-subscribed to receive email notifications."

### fn spec.initProvider.withBehaviors

```ts
withBehaviors(behaviors)
```

"A set of behaviors for a Microsoft 365 group. Possible values are AllowOnlyMembersToPost, HideGroupInOutlook, SkipExchangeInstantOn, SubscribeMembersToCalendarEventsDisabled, SubscribeNewGroupMembers and WelcomeEmailDisabled. See official documentation for more details. Changing this forces a new resource to be created.\nThe group behaviours for a Microsoft 365 group"

### fn spec.initProvider.withBehaviorsMixin

```ts
withBehaviorsMixin(behaviors)
```

"A set of behaviors for a Microsoft 365 group. Possible values are AllowOnlyMembersToPost, HideGroupInOutlook, SkipExchangeInstantOn, SubscribeMembersToCalendarEventsDisabled, SubscribeNewGroupMembers and WelcomeEmailDisabled. See official documentation for more details. Changing this forces a new resource to be created.\nThe group behaviours for a Microsoft 365 group"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withDescription

```ts
withDescription(description)
```

"The description for the group.\nThe description for the group"

### fn spec.initProvider.withDisplayName

```ts
withDisplayName(displayName)
```

"The display name for the group.\nThe display name for the group"

### fn spec.initProvider.withExternalSendersAllowed

```ts
withExternalSendersAllowed(externalSendersAllowed)
```

"Indicates whether people external to the organization can send messages to the group. Can only be set for Unified groups.\nIndicates whether people external to the organization can send messages to the group."

### fn spec.initProvider.withHideFromAddressLists

```ts
withHideFromAddressLists(hideFromAddressLists)
```

"Indicates whether the group is displayed in certain parts of the Outlook user interface: in the Address Book, in address lists for selecting message recipients, and in the Browse Groups dialog for searching groups. Can only be set for Unified groups.\nIndicates whether the group is displayed in certain parts of the Outlook user interface: in the Address Book, in address lists for selecting message recipients, and in the Browse Groups dialog for searching groups."

### fn spec.initProvider.withHideFromOutlookClients

```ts
withHideFromOutlookClients(hideFromOutlookClients)
```

"Indicates whether the group is displayed in Outlook clients, such as Outlook for Windows and Outlook on the web. Can only be set for Unified groups.\nIndicates whether the group is displayed in Outlook clients, such as Outlook for Windows and Outlook on the web."

### fn spec.initProvider.withMailEnabled

```ts
withMailEnabled(mailEnabled)
```

"Whether the group is a mail enabled, with a shared group mailbox. At least one of mail_enabled or security_enabled must be specified. Only Microsoft 365 groups can be mail enabled (see the types property).\nWhether the group is a mail enabled, with a shared group mailbox. At least one of `mail_enabled` or `security_enabled` must be specified. A group can be mail enabled _and_ security enabled"

### fn spec.initProvider.withMailNickname

```ts
withMailNickname(mailNickname)
```

"The mail alias for the group, unique in the organisation. Required for mail-enabled groups. Changing this forces a new resource to be created.\nThe mail alias for the group, unique in the organisation"

### fn spec.initProvider.withMembers

```ts
withMembers(members)
```

"A set of members who should be present in this group. Supported object types are Users, Groups or Service Principals. Cannot be used with the dynamic_membership block.\nA set of members who should be present in this group. Supported object types are Users, Groups or Service Principals"

### fn spec.initProvider.withMembersMixin

```ts
withMembersMixin(members)
```

"A set of members who should be present in this group. Supported object types are Users, Groups or Service Principals. Cannot be used with the dynamic_membership block.\nA set of members who should be present in this group. Supported object types are Users, Groups or Service Principals"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withMembersRefs

```ts
withMembersRefs(membersRefs)
```

"References to User in users to populate members."

### fn spec.initProvider.withMembersRefsMixin

```ts
withMembersRefsMixin(membersRefs)
```

"References to User in users to populate members."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withOnpremisesGroupType

```ts
withOnpremisesGroupType(onpremisesGroupType)
```

"The on-premises group type that the AAD group will be written as, when writeback is enabled. Possible values are UniversalDistributionGroup, UniversalMailEnabledSecurityGroup, or UniversalSecurityGroup.\nIndicates the target on-premise group type the group will be written back as"

### fn spec.initProvider.withOwners

```ts
withOwners(owners)
```

"A set of object IDs of principals that will be granted ownership of the group. Supported object types are users or service principals. Groups cannot be created with no owners or have all their owners removed.\nA set of owners who own this group. Supported object types are Users or Service Principals"

### fn spec.initProvider.withOwnersMixin

```ts
withOwnersMixin(owners)
```

"A set of object IDs of principals that will be granted ownership of the group. Supported object types are users or service principals. Groups cannot be created with no owners or have all their owners removed.\nA set of owners who own this group. Supported object types are Users or Service Principals"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withPreventDuplicateNames

```ts
withPreventDuplicateNames(preventDuplicateNames)
```

"If true, will return an error if an existing group is found with the same name. Defaults to false.\nIf `true`, will return an error if an existing group is found with the same name"

### fn spec.initProvider.withProvisioningOptions

```ts
withProvisioningOptions(provisioningOptions)
```

"A set of provisioning options for a Microsoft 365 group. The only supported value is Team. See official documentation for details. Changing this forces a new resource to be created.\nThe group provisioning options for a Microsoft 365 group"

### fn spec.initProvider.withProvisioningOptionsMixin

```ts
withProvisioningOptionsMixin(provisioningOptions)
```

"A set of provisioning options for a Microsoft 365 group. The only supported value is Team. See official documentation for details. Changing this forces a new resource to be created.\nThe group provisioning options for a Microsoft 365 group"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withSecurityEnabled

```ts
withSecurityEnabled(securityEnabled)
```

"Whether the group is a security group for controlling access to in-app resources. At least one of security_enabled or mail_enabled must be specified. A Microsoft 365 group can be security enabled and mail enabled (see the types property).\nWhether the group is a security group for controlling access to in-app resources. At least one of `security_enabled` or `mail_enabled` must be specified. A group can be security enabled _and_ mail enabled"

### fn spec.initProvider.withTheme

```ts
withTheme(theme)
```

"The colour theme for a Microsoft 365 group. Possible values are Blue, Green, Orange, Pink, Purple, Red or Teal. By default, no theme is set.\nThe colour theme for a Microsoft 365 group"

### fn spec.initProvider.withTypes

```ts
withTypes(types)
```

"A set of group types to configure for the group. Supported values are DynamicMembership, which denotes a group with dynamic membership, and Unified, which specifies a Microsoft 365 group. Required when mail_enabled is true. Changing this forces a new resource to be created.\nA set of group types to configure for the group. `Unified` specifies a Microsoft 365 group. Required when `mail_enabled` is true"

### fn spec.initProvider.withTypesMixin

```ts
withTypesMixin(types)
```

"A set of group types to configure for the group. Supported values are DynamicMembership, which denotes a group with dynamic membership, and Unified, which specifies a Microsoft 365 group. Required when mail_enabled is true. Changing this forces a new resource to be created.\nA set of group types to configure for the group. `Unified` specifies a Microsoft 365 group. Required when `mail_enabled` is true"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withVisibility

```ts
withVisibility(visibility)
```

"The group join policy and group content visibility. Possible values are Private, Public, or Hiddenmembership. Only Microsoft 365 groups can have Hiddenmembership visibility and this value must be set when the group is created. By default, security groups will receive Private visibility and Microsoft 365 groups will receive Public visibility.\nSpecifies the group join policy and group content visibility"

### fn spec.initProvider.withWritebackEnabled

```ts
withWritebackEnabled(writebackEnabled)
```

"Whether the group will be written back to the configured on-premises Active Directory when Azure AD Connect is used.\nWhether this group should be synced from Azure AD to the on-premises directory when Azure AD Connect is used"

## obj spec.initProvider.dynamicMembership

"A dynamic_membership block as documented below. Required when types contains DynamicMembership. Cannot be used with the members property.\nAn optional block to configure dynamic membership for the group. Cannot be used with `members`"

### fn spec.initProvider.dynamicMembership.withEnabled

```ts
withEnabled(enabled)
```

"Whether rule processing is \"On\" (true) or \"Paused\" (false)."

### fn spec.initProvider.dynamicMembership.withRule

```ts
withRule(rule)
```

"The rule that determines membership of this group. For more information, see official documentation on membership rules syntax.\nRule to determine members for a dynamic group. Required when `group_types` contains 'DynamicMembership'"

## obj spec.initProvider.membersRefs

"References to User in users to populate members."

### fn spec.initProvider.membersRefs.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.initProvider.membersRefs.policy

"Policies for referencing."

### fn spec.initProvider.membersRefs.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.initProvider.membersRefs.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.initProvider.membersSelector

"Selector for a list of User in users to populate members."

### fn spec.initProvider.membersSelector.withMatchControllerRef

```ts
withMatchControllerRef(matchControllerRef)
```

"MatchControllerRef ensures an object with the same controller reference\nas the selecting object is selected."

### fn spec.initProvider.membersSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

### fn spec.initProvider.membersSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.membersSelector.policy

"Policies for selection."

### fn spec.initProvider.membersSelector.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.initProvider.membersSelector.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.providerConfigRef

"ProviderConfigReference specifies how the provider that will be used to\ncreate, observe, update, and delete this managed resource should be\nconfigured."

### fn spec.providerConfigRef.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.providerConfigRef.policy

"Policies for referencing."

### fn spec.providerConfigRef.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.providerConfigRef.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.writeConnectionSecretToRef

"WriteConnectionSecretToReference specifies the namespace and name of a\nSecret to which any connection details for this managed resource should\nbe written. Connection details frequently include the endpoint, username,\nand password required to connect to the managed resource."

### fn spec.writeConnectionSecretToRef.withName

```ts
withName(name)
```

"Name of the secret."

### fn spec.writeConnectionSecretToRef.withNamespace

```ts
withNamespace(namespace)
```

"Namespace of the secret."