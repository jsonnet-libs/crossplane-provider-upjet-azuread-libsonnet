---
permalink: /upbound-provider-azuread/cluster/identitygovernance/v1beta1/privilegedAccessGroupEligibilitySchedule/
---

# identitygovernance.v1beta1.privilegedAccessGroupEligibilitySchedule

"PrivilegedAccessGroupEligibilitySchedule is the Schema for the PrivilegedAccessGroupEligibilitySchedules API."

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
    * [`fn withAssignmentType(assignmentType)`](#fn-specforproviderwithassignmenttype)
    * [`fn withDuration(duration)`](#fn-specforproviderwithduration)
    * [`fn withExpirationDate(expirationDate)`](#fn-specforproviderwithexpirationdate)
    * [`fn withGroupId(groupId)`](#fn-specforproviderwithgroupid)
    * [`fn withJustification(justification)`](#fn-specforproviderwithjustification)
    * [`fn withPermanentAssignment(permanentAssignment)`](#fn-specforproviderwithpermanentassignment)
    * [`fn withPrincipalId(principalId)`](#fn-specforproviderwithprincipalid)
    * [`fn withStartDate(startDate)`](#fn-specforproviderwithstartdate)
    * [`fn withTicketNumber(ticketNumber)`](#fn-specforproviderwithticketnumber)
    * [`fn withTicketSystem(ticketSystem)`](#fn-specforproviderwithticketsystem)
    * [`obj spec.forProvider.groupIdRef`](#obj-specforprovidergroupidref)
      * [`fn withName(name)`](#fn-specforprovidergroupidrefwithname)
      * [`obj spec.forProvider.groupIdRef.policy`](#obj-specforprovidergroupidrefpolicy)
        * [`fn withResolution(resolution)`](#fn-specforprovidergroupidrefpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specforprovidergroupidrefpolicywithresolve)
    * [`obj spec.forProvider.groupIdSelector`](#obj-specforprovidergroupidselector)
      * [`fn withMatchControllerRef(matchControllerRef)`](#fn-specforprovidergroupidselectorwithmatchcontrollerref)
      * [`fn withMatchLabels(matchLabels)`](#fn-specforprovidergroupidselectorwithmatchlabels)
      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specforprovidergroupidselectorwithmatchlabelsmixin)
      * [`obj spec.forProvider.groupIdSelector.policy`](#obj-specforprovidergroupidselectorpolicy)
        * [`fn withResolution(resolution)`](#fn-specforprovidergroupidselectorpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specforprovidergroupidselectorpolicywithresolve)
    * [`obj spec.forProvider.principalIdRef`](#obj-specforproviderprincipalidref)
      * [`fn withName(name)`](#fn-specforproviderprincipalidrefwithname)
      * [`obj spec.forProvider.principalIdRef.policy`](#obj-specforproviderprincipalidrefpolicy)
        * [`fn withResolution(resolution)`](#fn-specforproviderprincipalidrefpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specforproviderprincipalidrefpolicywithresolve)
    * [`obj spec.forProvider.principalIdSelector`](#obj-specforproviderprincipalidselector)
      * [`fn withMatchControllerRef(matchControllerRef)`](#fn-specforproviderprincipalidselectorwithmatchcontrollerref)
      * [`fn withMatchLabels(matchLabels)`](#fn-specforproviderprincipalidselectorwithmatchlabels)
      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specforproviderprincipalidselectorwithmatchlabelsmixin)
      * [`obj spec.forProvider.principalIdSelector.policy`](#obj-specforproviderprincipalidselectorpolicy)
        * [`fn withResolution(resolution)`](#fn-specforproviderprincipalidselectorpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specforproviderprincipalidselectorpolicywithresolve)
  * [`obj spec.initProvider`](#obj-specinitprovider)
    * [`fn withAssignmentType(assignmentType)`](#fn-specinitproviderwithassignmenttype)
    * [`fn withDuration(duration)`](#fn-specinitproviderwithduration)
    * [`fn withExpirationDate(expirationDate)`](#fn-specinitproviderwithexpirationdate)
    * [`fn withGroupId(groupId)`](#fn-specinitproviderwithgroupid)
    * [`fn withJustification(justification)`](#fn-specinitproviderwithjustification)
    * [`fn withPermanentAssignment(permanentAssignment)`](#fn-specinitproviderwithpermanentassignment)
    * [`fn withPrincipalId(principalId)`](#fn-specinitproviderwithprincipalid)
    * [`fn withStartDate(startDate)`](#fn-specinitproviderwithstartdate)
    * [`fn withTicketNumber(ticketNumber)`](#fn-specinitproviderwithticketnumber)
    * [`fn withTicketSystem(ticketSystem)`](#fn-specinitproviderwithticketsystem)
    * [`obj spec.initProvider.groupIdRef`](#obj-specinitprovidergroupidref)
      * [`fn withName(name)`](#fn-specinitprovidergroupidrefwithname)
      * [`obj spec.initProvider.groupIdRef.policy`](#obj-specinitprovidergroupidrefpolicy)
        * [`fn withResolution(resolution)`](#fn-specinitprovidergroupidrefpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specinitprovidergroupidrefpolicywithresolve)
    * [`obj spec.initProvider.groupIdSelector`](#obj-specinitprovidergroupidselector)
      * [`fn withMatchControllerRef(matchControllerRef)`](#fn-specinitprovidergroupidselectorwithmatchcontrollerref)
      * [`fn withMatchLabels(matchLabels)`](#fn-specinitprovidergroupidselectorwithmatchlabels)
      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specinitprovidergroupidselectorwithmatchlabelsmixin)
      * [`obj spec.initProvider.groupIdSelector.policy`](#obj-specinitprovidergroupidselectorpolicy)
        * [`fn withResolution(resolution)`](#fn-specinitprovidergroupidselectorpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specinitprovidergroupidselectorpolicywithresolve)
    * [`obj spec.initProvider.principalIdRef`](#obj-specinitproviderprincipalidref)
      * [`fn withName(name)`](#fn-specinitproviderprincipalidrefwithname)
      * [`obj spec.initProvider.principalIdRef.policy`](#obj-specinitproviderprincipalidrefpolicy)
        * [`fn withResolution(resolution)`](#fn-specinitproviderprincipalidrefpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specinitproviderprincipalidrefpolicywithresolve)
    * [`obj spec.initProvider.principalIdSelector`](#obj-specinitproviderprincipalidselector)
      * [`fn withMatchControllerRef(matchControllerRef)`](#fn-specinitproviderprincipalidselectorwithmatchcontrollerref)
      * [`fn withMatchLabels(matchLabels)`](#fn-specinitproviderprincipalidselectorwithmatchlabels)
      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specinitproviderprincipalidselectorwithmatchlabelsmixin)
      * [`obj spec.initProvider.principalIdSelector.policy`](#obj-specinitproviderprincipalidselectorpolicy)
        * [`fn withResolution(resolution)`](#fn-specinitproviderprincipalidselectorpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specinitproviderprincipalidselectorpolicywithresolve)
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

new returns an instance of PrivilegedAccessGroupEligibilitySchedule

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

"PrivilegedAccessGroupEligibilityScheduleSpec defines the desired state of PrivilegedAccessGroupEligibilitySchedule"

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



### fn spec.forProvider.withAssignmentType

```ts
withAssignmentType(assignmentType)
```

"The type of assignment to the group. Can be either member or owner.\nThe ID of the assignment to the group"

### fn spec.forProvider.withDuration

```ts
withDuration(duration)
```

"The duration that this assignment is valid for, formatted as an ISO8601 duration (e.g. P30D for 30 days, PT3H for three hours).\nThe duration of the assignment, formatted as an ISO8601 duration string (e.g. P3D for 3 days)"

### fn spec.forProvider.withExpirationDate

```ts
withExpirationDate(expirationDate)
```

"01-01T01:02:03Z).\nThe date that this assignment expires, formatted as an RFC3339 date string in UTC (e.g. 2018-01-01T01:02:03Z)"

### fn spec.forProvider.withGroupId

```ts
withGroupId(groupId)
```

"The Object ID of the Azure AD group to which the principal will be assigned.\nThe ID of the Group representing the scope of the assignment"

### fn spec.forProvider.withJustification

```ts
withJustification(justification)
```

"The justification for this assignment. May be required by the role policy.\nThe justification for the assignment"

### fn spec.forProvider.withPermanentAssignment

```ts
withPermanentAssignment(permanentAssignment)
```

"Is this assigment permanently valid.\nIs the assignment permanent"

### fn spec.forProvider.withPrincipalId

```ts
withPrincipalId(principalId)
```

"The Object ID of the principal to be assigned to the above group. Can be either a user or a group.\nThe ID of the Principal assigned to the schedule"

### fn spec.forProvider.withStartDate

```ts
withStartDate(startDate)
```

"01-01T01:02:03Z). If not provided, the assignment is immediately valid.\nThe date that this assignment starts, formatted as an RFC3339 date string in UTC (e.g. 2018-01-01T01:02:03Z)"

### fn spec.forProvider.withTicketNumber

```ts
withTicketNumber(ticketNumber)
```

"The ticket number in the ticket system approving this assignment. May be required by the role policy.\nThe ticket number authorising the assignment"

### fn spec.forProvider.withTicketSystem

```ts
withTicketSystem(ticketSystem)
```

"The ticket system containing the ticket number approving this assignment. May be required by the role policy.\nThe ticket system authorising the assignment"

## obj spec.forProvider.groupIdRef

"Reference to a Group in groups to populate groupId."

### fn spec.forProvider.groupIdRef.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.forProvider.groupIdRef.policy

"Policies for referencing."

### fn spec.forProvider.groupIdRef.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.forProvider.groupIdRef.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.forProvider.groupIdSelector

"Selector for a Group in groups to populate groupId."

### fn spec.forProvider.groupIdSelector.withMatchControllerRef

```ts
withMatchControllerRef(matchControllerRef)
```

"MatchControllerRef ensures an object with the same controller reference\nas the selecting object is selected."

### fn spec.forProvider.groupIdSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

### fn spec.forProvider.groupIdSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.groupIdSelector.policy

"Policies for selection."

### fn spec.forProvider.groupIdSelector.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.forProvider.groupIdSelector.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.forProvider.principalIdRef

"Reference to a User in users to populate principalId."

### fn spec.forProvider.principalIdRef.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.forProvider.principalIdRef.policy

"Policies for referencing."

### fn spec.forProvider.principalIdRef.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.forProvider.principalIdRef.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.forProvider.principalIdSelector

"Selector for a User in users to populate principalId."

### fn spec.forProvider.principalIdSelector.withMatchControllerRef

```ts
withMatchControllerRef(matchControllerRef)
```

"MatchControllerRef ensures an object with the same controller reference\nas the selecting object is selected."

### fn spec.forProvider.principalIdSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

### fn spec.forProvider.principalIdSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.principalIdSelector.policy

"Policies for selection."

### fn spec.forProvider.principalIdSelector.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.forProvider.principalIdSelector.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.initProvider

"THIS IS A BETA FIELD. It will be honored\nunless the Management Policies feature flag is disabled.\nInitProvider holds the same fields as ForProvider, with the exception\nof Identifier and other resource reference fields. The fields that are\nin InitProvider are merged into ForProvider when the resource is created.\nThe same fields are also added to the terraform ignore_changes hook, to\navoid updating them after creation. This is useful for fields that are\nrequired on creation, but we do not desire to update them after creation,\nfor example because of an external controller is managing them, like an\nautoscaler."

### fn spec.initProvider.withAssignmentType

```ts
withAssignmentType(assignmentType)
```

"The type of assignment to the group. Can be either member or owner.\nThe ID of the assignment to the group"

### fn spec.initProvider.withDuration

```ts
withDuration(duration)
```

"The duration that this assignment is valid for, formatted as an ISO8601 duration (e.g. P30D for 30 days, PT3H for three hours).\nThe duration of the assignment, formatted as an ISO8601 duration string (e.g. P3D for 3 days)"

### fn spec.initProvider.withExpirationDate

```ts
withExpirationDate(expirationDate)
```

"01-01T01:02:03Z).\nThe date that this assignment expires, formatted as an RFC3339 date string in UTC (e.g. 2018-01-01T01:02:03Z)"

### fn spec.initProvider.withGroupId

```ts
withGroupId(groupId)
```

"The Object ID of the Azure AD group to which the principal will be assigned.\nThe ID of the Group representing the scope of the assignment"

### fn spec.initProvider.withJustification

```ts
withJustification(justification)
```

"The justification for this assignment. May be required by the role policy.\nThe justification for the assignment"

### fn spec.initProvider.withPermanentAssignment

```ts
withPermanentAssignment(permanentAssignment)
```

"Is this assigment permanently valid.\nIs the assignment permanent"

### fn spec.initProvider.withPrincipalId

```ts
withPrincipalId(principalId)
```

"The Object ID of the principal to be assigned to the above group. Can be either a user or a group.\nThe ID of the Principal assigned to the schedule"

### fn spec.initProvider.withStartDate

```ts
withStartDate(startDate)
```

"01-01T01:02:03Z). If not provided, the assignment is immediately valid.\nThe date that this assignment starts, formatted as an RFC3339 date string in UTC (e.g. 2018-01-01T01:02:03Z)"

### fn spec.initProvider.withTicketNumber

```ts
withTicketNumber(ticketNumber)
```

"The ticket number in the ticket system approving this assignment. May be required by the role policy.\nThe ticket number authorising the assignment"

### fn spec.initProvider.withTicketSystem

```ts
withTicketSystem(ticketSystem)
```

"The ticket system containing the ticket number approving this assignment. May be required by the role policy.\nThe ticket system authorising the assignment"

## obj spec.initProvider.groupIdRef

"Reference to a Group in groups to populate groupId."

### fn spec.initProvider.groupIdRef.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.initProvider.groupIdRef.policy

"Policies for referencing."

### fn spec.initProvider.groupIdRef.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.initProvider.groupIdRef.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.initProvider.groupIdSelector

"Selector for a Group in groups to populate groupId."

### fn spec.initProvider.groupIdSelector.withMatchControllerRef

```ts
withMatchControllerRef(matchControllerRef)
```

"MatchControllerRef ensures an object with the same controller reference\nas the selecting object is selected."

### fn spec.initProvider.groupIdSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

### fn spec.initProvider.groupIdSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.groupIdSelector.policy

"Policies for selection."

### fn spec.initProvider.groupIdSelector.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.initProvider.groupIdSelector.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.initProvider.principalIdRef

"Reference to a User in users to populate principalId."

### fn spec.initProvider.principalIdRef.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.initProvider.principalIdRef.policy

"Policies for referencing."

### fn spec.initProvider.principalIdRef.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.initProvider.principalIdRef.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.initProvider.principalIdSelector

"Selector for a User in users to populate principalId."

### fn spec.initProvider.principalIdSelector.withMatchControllerRef

```ts
withMatchControllerRef(matchControllerRef)
```

"MatchControllerRef ensures an object with the same controller reference\nas the selecting object is selected."

### fn spec.initProvider.principalIdSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

### fn spec.initProvider.principalIdSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.principalIdSelector.policy

"Policies for selection."

### fn spec.initProvider.principalIdSelector.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.initProvider.principalIdSelector.policy.withResolve

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