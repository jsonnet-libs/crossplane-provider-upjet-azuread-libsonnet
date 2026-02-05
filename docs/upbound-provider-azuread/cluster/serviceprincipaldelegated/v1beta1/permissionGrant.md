---
permalink: /upbound-provider-azuread/cluster/serviceprincipaldelegated/v1beta1/permissionGrant/
---

# serviceprincipaldelegated.v1beta1.permissionGrant

"PermissionGrant is the Schema for the PermissionGrants API."

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
    * [`fn withClaimValues(claimValues)`](#fn-specforproviderwithclaimvalues)
    * [`fn withClaimValuesMixin(claimValues)`](#fn-specforproviderwithclaimvaluesmixin)
    * [`fn withResourceServicePrincipalObjectId(resourceServicePrincipalObjectId)`](#fn-specforproviderwithresourceserviceprincipalobjectid)
    * [`fn withServicePrincipalObjectId(servicePrincipalObjectId)`](#fn-specforproviderwithserviceprincipalobjectid)
    * [`fn withUserObjectId(userObjectId)`](#fn-specforproviderwithuserobjectid)
    * [`obj spec.forProvider.resourceServicePrincipalObjectIdRef`](#obj-specforproviderresourceserviceprincipalobjectidref)
      * [`fn withName(name)`](#fn-specforproviderresourceserviceprincipalobjectidrefwithname)
      * [`obj spec.forProvider.resourceServicePrincipalObjectIdRef.policy`](#obj-specforproviderresourceserviceprincipalobjectidrefpolicy)
        * [`fn withResolution(resolution)`](#fn-specforproviderresourceserviceprincipalobjectidrefpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specforproviderresourceserviceprincipalobjectidrefpolicywithresolve)
    * [`obj spec.forProvider.resourceServicePrincipalObjectIdSelector`](#obj-specforproviderresourceserviceprincipalobjectidselector)
      * [`fn withMatchControllerRef(matchControllerRef)`](#fn-specforproviderresourceserviceprincipalobjectidselectorwithmatchcontrollerref)
      * [`fn withMatchLabels(matchLabels)`](#fn-specforproviderresourceserviceprincipalobjectidselectorwithmatchlabels)
      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specforproviderresourceserviceprincipalobjectidselectorwithmatchlabelsmixin)
      * [`obj spec.forProvider.resourceServicePrincipalObjectIdSelector.policy`](#obj-specforproviderresourceserviceprincipalobjectidselectorpolicy)
        * [`fn withResolution(resolution)`](#fn-specforproviderresourceserviceprincipalobjectidselectorpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specforproviderresourceserviceprincipalobjectidselectorpolicywithresolve)
    * [`obj spec.forProvider.servicePrincipalObjectIdRef`](#obj-specforproviderserviceprincipalobjectidref)
      * [`fn withName(name)`](#fn-specforproviderserviceprincipalobjectidrefwithname)
      * [`obj spec.forProvider.servicePrincipalObjectIdRef.policy`](#obj-specforproviderserviceprincipalobjectidrefpolicy)
        * [`fn withResolution(resolution)`](#fn-specforproviderserviceprincipalobjectidrefpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specforproviderserviceprincipalobjectidrefpolicywithresolve)
    * [`obj spec.forProvider.servicePrincipalObjectIdSelector`](#obj-specforproviderserviceprincipalobjectidselector)
      * [`fn withMatchControllerRef(matchControllerRef)`](#fn-specforproviderserviceprincipalobjectidselectorwithmatchcontrollerref)
      * [`fn withMatchLabels(matchLabels)`](#fn-specforproviderserviceprincipalobjectidselectorwithmatchlabels)
      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specforproviderserviceprincipalobjectidselectorwithmatchlabelsmixin)
      * [`obj spec.forProvider.servicePrincipalObjectIdSelector.policy`](#obj-specforproviderserviceprincipalobjectidselectorpolicy)
        * [`fn withResolution(resolution)`](#fn-specforproviderserviceprincipalobjectidselectorpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specforproviderserviceprincipalobjectidselectorpolicywithresolve)
    * [`obj spec.forProvider.userObjectIdRef`](#obj-specforprovideruserobjectidref)
      * [`fn withName(name)`](#fn-specforprovideruserobjectidrefwithname)
      * [`obj spec.forProvider.userObjectIdRef.policy`](#obj-specforprovideruserobjectidrefpolicy)
        * [`fn withResolution(resolution)`](#fn-specforprovideruserobjectidrefpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specforprovideruserobjectidrefpolicywithresolve)
    * [`obj spec.forProvider.userObjectIdSelector`](#obj-specforprovideruserobjectidselector)
      * [`fn withMatchControllerRef(matchControllerRef)`](#fn-specforprovideruserobjectidselectorwithmatchcontrollerref)
      * [`fn withMatchLabels(matchLabels)`](#fn-specforprovideruserobjectidselectorwithmatchlabels)
      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specforprovideruserobjectidselectorwithmatchlabelsmixin)
      * [`obj spec.forProvider.userObjectIdSelector.policy`](#obj-specforprovideruserobjectidselectorpolicy)
        * [`fn withResolution(resolution)`](#fn-specforprovideruserobjectidselectorpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specforprovideruserobjectidselectorpolicywithresolve)
  * [`obj spec.initProvider`](#obj-specinitprovider)
    * [`fn withClaimValues(claimValues)`](#fn-specinitproviderwithclaimvalues)
    * [`fn withClaimValuesMixin(claimValues)`](#fn-specinitproviderwithclaimvaluesmixin)
    * [`fn withResourceServicePrincipalObjectId(resourceServicePrincipalObjectId)`](#fn-specinitproviderwithresourceserviceprincipalobjectid)
    * [`fn withServicePrincipalObjectId(servicePrincipalObjectId)`](#fn-specinitproviderwithserviceprincipalobjectid)
    * [`fn withUserObjectId(userObjectId)`](#fn-specinitproviderwithuserobjectid)
    * [`obj spec.initProvider.resourceServicePrincipalObjectIdRef`](#obj-specinitproviderresourceserviceprincipalobjectidref)
      * [`fn withName(name)`](#fn-specinitproviderresourceserviceprincipalobjectidrefwithname)
      * [`obj spec.initProvider.resourceServicePrincipalObjectIdRef.policy`](#obj-specinitproviderresourceserviceprincipalobjectidrefpolicy)
        * [`fn withResolution(resolution)`](#fn-specinitproviderresourceserviceprincipalobjectidrefpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specinitproviderresourceserviceprincipalobjectidrefpolicywithresolve)
    * [`obj spec.initProvider.resourceServicePrincipalObjectIdSelector`](#obj-specinitproviderresourceserviceprincipalobjectidselector)
      * [`fn withMatchControllerRef(matchControllerRef)`](#fn-specinitproviderresourceserviceprincipalobjectidselectorwithmatchcontrollerref)
      * [`fn withMatchLabels(matchLabels)`](#fn-specinitproviderresourceserviceprincipalobjectidselectorwithmatchlabels)
      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specinitproviderresourceserviceprincipalobjectidselectorwithmatchlabelsmixin)
      * [`obj spec.initProvider.resourceServicePrincipalObjectIdSelector.policy`](#obj-specinitproviderresourceserviceprincipalobjectidselectorpolicy)
        * [`fn withResolution(resolution)`](#fn-specinitproviderresourceserviceprincipalobjectidselectorpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specinitproviderresourceserviceprincipalobjectidselectorpolicywithresolve)
    * [`obj spec.initProvider.servicePrincipalObjectIdRef`](#obj-specinitproviderserviceprincipalobjectidref)
      * [`fn withName(name)`](#fn-specinitproviderserviceprincipalobjectidrefwithname)
      * [`obj spec.initProvider.servicePrincipalObjectIdRef.policy`](#obj-specinitproviderserviceprincipalobjectidrefpolicy)
        * [`fn withResolution(resolution)`](#fn-specinitproviderserviceprincipalobjectidrefpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specinitproviderserviceprincipalobjectidrefpolicywithresolve)
    * [`obj spec.initProvider.servicePrincipalObjectIdSelector`](#obj-specinitproviderserviceprincipalobjectidselector)
      * [`fn withMatchControllerRef(matchControllerRef)`](#fn-specinitproviderserviceprincipalobjectidselectorwithmatchcontrollerref)
      * [`fn withMatchLabels(matchLabels)`](#fn-specinitproviderserviceprincipalobjectidselectorwithmatchlabels)
      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specinitproviderserviceprincipalobjectidselectorwithmatchlabelsmixin)
      * [`obj spec.initProvider.servicePrincipalObjectIdSelector.policy`](#obj-specinitproviderserviceprincipalobjectidselectorpolicy)
        * [`fn withResolution(resolution)`](#fn-specinitproviderserviceprincipalobjectidselectorpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specinitproviderserviceprincipalobjectidselectorpolicywithresolve)
    * [`obj spec.initProvider.userObjectIdRef`](#obj-specinitprovideruserobjectidref)
      * [`fn withName(name)`](#fn-specinitprovideruserobjectidrefwithname)
      * [`obj spec.initProvider.userObjectIdRef.policy`](#obj-specinitprovideruserobjectidrefpolicy)
        * [`fn withResolution(resolution)`](#fn-specinitprovideruserobjectidrefpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specinitprovideruserobjectidrefpolicywithresolve)
    * [`obj spec.initProvider.userObjectIdSelector`](#obj-specinitprovideruserobjectidselector)
      * [`fn withMatchControllerRef(matchControllerRef)`](#fn-specinitprovideruserobjectidselectorwithmatchcontrollerref)
      * [`fn withMatchLabels(matchLabels)`](#fn-specinitprovideruserobjectidselectorwithmatchlabels)
      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specinitprovideruserobjectidselectorwithmatchlabelsmixin)
      * [`obj spec.initProvider.userObjectIdSelector.policy`](#obj-specinitprovideruserobjectidselectorpolicy)
        * [`fn withResolution(resolution)`](#fn-specinitprovideruserobjectidselectorpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specinitprovideruserobjectidselectorpolicywithresolve)
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

new returns an instance of PermissionGrant

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

"PermissionGrantSpec defines the desired state of PermissionGrant"

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



### fn spec.forProvider.withClaimValues

```ts
withClaimValues(claimValues)
```

"- A set of claim values for delegated permission scopes which should be included in access tokens for the resource.\nA set of claim values for delegated permission scopes which should be included in access tokens for the resource"

### fn spec.forProvider.withClaimValuesMixin

```ts
withClaimValuesMixin(claimValues)
```

"- A set of claim values for delegated permission scopes which should be included in access tokens for the resource.\nA set of claim values for delegated permission scopes which should be included in access tokens for the resource"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withResourceServicePrincipalObjectId

```ts
withResourceServicePrincipalObjectId(resourceServicePrincipalObjectId)
```

"The object ID of the service principal representing the resource to be accessed. Changing this forces a new resource to be created.\nThe object ID of the service principal representing the resource to be accessed"

### fn spec.forProvider.withServicePrincipalObjectId

```ts
withServicePrincipalObjectId(servicePrincipalObjectId)
```

"The object ID of the service principal for which this delegated permission grant should be created. Changing this forces a new resource to be created.\nThe object ID of the service principal for which this delegated permission grant should be created"

### fn spec.forProvider.withUserObjectId

```ts
withUserObjectId(userObjectId)
```

"- The object ID of the user on behalf of whom the service principal is authorized to access the resource. When omitted, the delegated permission grant will be consented for all users. Changing this forces a new resource to be created.\nThe object ID of the user on behalf of whom the service principal is authorized to access the resource"

## obj spec.forProvider.resourceServicePrincipalObjectIdRef

"Reference to a Principal in serviceprincipals to populate resourceServicePrincipalObjectId."

### fn spec.forProvider.resourceServicePrincipalObjectIdRef.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.forProvider.resourceServicePrincipalObjectIdRef.policy

"Policies for referencing."

### fn spec.forProvider.resourceServicePrincipalObjectIdRef.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.forProvider.resourceServicePrincipalObjectIdRef.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.forProvider.resourceServicePrincipalObjectIdSelector

"Selector for a Principal in serviceprincipals to populate resourceServicePrincipalObjectId."

### fn spec.forProvider.resourceServicePrincipalObjectIdSelector.withMatchControllerRef

```ts
withMatchControllerRef(matchControllerRef)
```

"MatchControllerRef ensures an object with the same controller reference\nas the selecting object is selected."

### fn spec.forProvider.resourceServicePrincipalObjectIdSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

### fn spec.forProvider.resourceServicePrincipalObjectIdSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.resourceServicePrincipalObjectIdSelector.policy

"Policies for selection."

### fn spec.forProvider.resourceServicePrincipalObjectIdSelector.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.forProvider.resourceServicePrincipalObjectIdSelector.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.forProvider.servicePrincipalObjectIdRef

"Reference to a Principal in serviceprincipals to populate servicePrincipalObjectId."

### fn spec.forProvider.servicePrincipalObjectIdRef.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.forProvider.servicePrincipalObjectIdRef.policy

"Policies for referencing."

### fn spec.forProvider.servicePrincipalObjectIdRef.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.forProvider.servicePrincipalObjectIdRef.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.forProvider.servicePrincipalObjectIdSelector

"Selector for a Principal in serviceprincipals to populate servicePrincipalObjectId."

### fn spec.forProvider.servicePrincipalObjectIdSelector.withMatchControllerRef

```ts
withMatchControllerRef(matchControllerRef)
```

"MatchControllerRef ensures an object with the same controller reference\nas the selecting object is selected."

### fn spec.forProvider.servicePrincipalObjectIdSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

### fn spec.forProvider.servicePrincipalObjectIdSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.servicePrincipalObjectIdSelector.policy

"Policies for selection."

### fn spec.forProvider.servicePrincipalObjectIdSelector.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.forProvider.servicePrincipalObjectIdSelector.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.forProvider.userObjectIdRef

"Reference to a User in users to populate userObjectId."

### fn spec.forProvider.userObjectIdRef.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.forProvider.userObjectIdRef.policy

"Policies for referencing."

### fn spec.forProvider.userObjectIdRef.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.forProvider.userObjectIdRef.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.forProvider.userObjectIdSelector

"Selector for a User in users to populate userObjectId."

### fn spec.forProvider.userObjectIdSelector.withMatchControllerRef

```ts
withMatchControllerRef(matchControllerRef)
```

"MatchControllerRef ensures an object with the same controller reference\nas the selecting object is selected."

### fn spec.forProvider.userObjectIdSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

### fn spec.forProvider.userObjectIdSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.userObjectIdSelector.policy

"Policies for selection."

### fn spec.forProvider.userObjectIdSelector.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.forProvider.userObjectIdSelector.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.initProvider

"THIS IS A BETA FIELD. It will be honored\nunless the Management Policies feature flag is disabled.\nInitProvider holds the same fields as ForProvider, with the exception\nof Identifier and other resource reference fields. The fields that are\nin InitProvider are merged into ForProvider when the resource is created.\nThe same fields are also added to the terraform ignore_changes hook, to\navoid updating them after creation. This is useful for fields that are\nrequired on creation, but we do not desire to update them after creation,\nfor example because of an external controller is managing them, like an\nautoscaler."

### fn spec.initProvider.withClaimValues

```ts
withClaimValues(claimValues)
```

"- A set of claim values for delegated permission scopes which should be included in access tokens for the resource.\nA set of claim values for delegated permission scopes which should be included in access tokens for the resource"

### fn spec.initProvider.withClaimValuesMixin

```ts
withClaimValuesMixin(claimValues)
```

"- A set of claim values for delegated permission scopes which should be included in access tokens for the resource.\nA set of claim values for delegated permission scopes which should be included in access tokens for the resource"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withResourceServicePrincipalObjectId

```ts
withResourceServicePrincipalObjectId(resourceServicePrincipalObjectId)
```

"The object ID of the service principal representing the resource to be accessed. Changing this forces a new resource to be created.\nThe object ID of the service principal representing the resource to be accessed"

### fn spec.initProvider.withServicePrincipalObjectId

```ts
withServicePrincipalObjectId(servicePrincipalObjectId)
```

"The object ID of the service principal for which this delegated permission grant should be created. Changing this forces a new resource to be created.\nThe object ID of the service principal for which this delegated permission grant should be created"

### fn spec.initProvider.withUserObjectId

```ts
withUserObjectId(userObjectId)
```

"- The object ID of the user on behalf of whom the service principal is authorized to access the resource. When omitted, the delegated permission grant will be consented for all users. Changing this forces a new resource to be created.\nThe object ID of the user on behalf of whom the service principal is authorized to access the resource"

## obj spec.initProvider.resourceServicePrincipalObjectIdRef

"Reference to a Principal in serviceprincipals to populate resourceServicePrincipalObjectId."

### fn spec.initProvider.resourceServicePrincipalObjectIdRef.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.initProvider.resourceServicePrincipalObjectIdRef.policy

"Policies for referencing."

### fn spec.initProvider.resourceServicePrincipalObjectIdRef.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.initProvider.resourceServicePrincipalObjectIdRef.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.initProvider.resourceServicePrincipalObjectIdSelector

"Selector for a Principal in serviceprincipals to populate resourceServicePrincipalObjectId."

### fn spec.initProvider.resourceServicePrincipalObjectIdSelector.withMatchControllerRef

```ts
withMatchControllerRef(matchControllerRef)
```

"MatchControllerRef ensures an object with the same controller reference\nas the selecting object is selected."

### fn spec.initProvider.resourceServicePrincipalObjectIdSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

### fn spec.initProvider.resourceServicePrincipalObjectIdSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.resourceServicePrincipalObjectIdSelector.policy

"Policies for selection."

### fn spec.initProvider.resourceServicePrincipalObjectIdSelector.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.initProvider.resourceServicePrincipalObjectIdSelector.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.initProvider.servicePrincipalObjectIdRef

"Reference to a Principal in serviceprincipals to populate servicePrincipalObjectId."

### fn spec.initProvider.servicePrincipalObjectIdRef.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.initProvider.servicePrincipalObjectIdRef.policy

"Policies for referencing."

### fn spec.initProvider.servicePrincipalObjectIdRef.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.initProvider.servicePrincipalObjectIdRef.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.initProvider.servicePrincipalObjectIdSelector

"Selector for a Principal in serviceprincipals to populate servicePrincipalObjectId."

### fn spec.initProvider.servicePrincipalObjectIdSelector.withMatchControllerRef

```ts
withMatchControllerRef(matchControllerRef)
```

"MatchControllerRef ensures an object with the same controller reference\nas the selecting object is selected."

### fn spec.initProvider.servicePrincipalObjectIdSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

### fn spec.initProvider.servicePrincipalObjectIdSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.servicePrincipalObjectIdSelector.policy

"Policies for selection."

### fn spec.initProvider.servicePrincipalObjectIdSelector.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.initProvider.servicePrincipalObjectIdSelector.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.initProvider.userObjectIdRef

"Reference to a User in users to populate userObjectId."

### fn spec.initProvider.userObjectIdRef.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.initProvider.userObjectIdRef.policy

"Policies for referencing."

### fn spec.initProvider.userObjectIdRef.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.initProvider.userObjectIdRef.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.initProvider.userObjectIdSelector

"Selector for a User in users to populate userObjectId."

### fn spec.initProvider.userObjectIdSelector.withMatchControllerRef

```ts
withMatchControllerRef(matchControllerRef)
```

"MatchControllerRef ensures an object with the same controller reference\nas the selecting object is selected."

### fn spec.initProvider.userObjectIdSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

### fn spec.initProvider.userObjectIdSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.userObjectIdSelector.policy

"Policies for selection."

### fn spec.initProvider.userObjectIdSelector.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.initProvider.userObjectIdSelector.policy.withResolve

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