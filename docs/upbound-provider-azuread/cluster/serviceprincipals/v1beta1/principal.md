---
permalink: /upbound-provider-azuread/cluster/serviceprincipals/v1beta1/principal/
---

# serviceprincipals.v1beta1.principal

"Principal is the Schema for the Principals API."

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
    * [`fn withAccountEnabled(accountEnabled)`](#fn-specforproviderwithaccountenabled)
    * [`fn withAlternativeNames(alternativeNames)`](#fn-specforproviderwithalternativenames)
    * [`fn withAlternativeNamesMixin(alternativeNames)`](#fn-specforproviderwithalternativenamesmixin)
    * [`fn withAppRoleAssignmentRequired(appRoleAssignmentRequired)`](#fn-specforproviderwithapproleassignmentrequired)
    * [`fn withClientId(clientId)`](#fn-specforproviderwithclientid)
    * [`fn withDescription(description)`](#fn-specforproviderwithdescription)
    * [`fn withFeatureTags(featureTags)`](#fn-specforproviderwithfeaturetags)
    * [`fn withFeatureTagsMixin(featureTags)`](#fn-specforproviderwithfeaturetagsmixin)
    * [`fn withLoginUrl(loginUrl)`](#fn-specforproviderwithloginurl)
    * [`fn withNotes(notes)`](#fn-specforproviderwithnotes)
    * [`fn withNotificationEmailAddresses(notificationEmailAddresses)`](#fn-specforproviderwithnotificationemailaddresses)
    * [`fn withNotificationEmailAddressesMixin(notificationEmailAddresses)`](#fn-specforproviderwithnotificationemailaddressesmixin)
    * [`fn withOwners(owners)`](#fn-specforproviderwithowners)
    * [`fn withOwnersMixin(owners)`](#fn-specforproviderwithownersmixin)
    * [`fn withPreferredSingleSignOnMode(preferredSingleSignOnMode)`](#fn-specforproviderwithpreferredsinglesignonmode)
    * [`fn withSamlSingleSignOn(samlSingleSignOn)`](#fn-specforproviderwithsamlsinglesignon)
    * [`fn withSamlSingleSignOnMixin(samlSingleSignOn)`](#fn-specforproviderwithsamlsinglesignonmixin)
    * [`fn withTags(tags)`](#fn-specforproviderwithtags)
    * [`fn withTagsMixin(tags)`](#fn-specforproviderwithtagsmixin)
    * [`fn withUseExisting(useExisting)`](#fn-specforproviderwithuseexisting)
    * [`obj spec.forProvider.clientIdRef`](#obj-specforproviderclientidref)
      * [`fn withName(name)`](#fn-specforproviderclientidrefwithname)
      * [`obj spec.forProvider.clientIdRef.policy`](#obj-specforproviderclientidrefpolicy)
        * [`fn withResolution(resolution)`](#fn-specforproviderclientidrefpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specforproviderclientidrefpolicywithresolve)
    * [`obj spec.forProvider.clientIdSelector`](#obj-specforproviderclientidselector)
      * [`fn withMatchControllerRef(matchControllerRef)`](#fn-specforproviderclientidselectorwithmatchcontrollerref)
      * [`fn withMatchLabels(matchLabels)`](#fn-specforproviderclientidselectorwithmatchlabels)
      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specforproviderclientidselectorwithmatchlabelsmixin)
      * [`obj spec.forProvider.clientIdSelector.policy`](#obj-specforproviderclientidselectorpolicy)
        * [`fn withResolution(resolution)`](#fn-specforproviderclientidselectorpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specforproviderclientidselectorpolicywithresolve)
    * [`obj spec.forProvider.featureTags`](#obj-specforproviderfeaturetags)
      * [`fn withCustomSingleSignOn(customSingleSignOn)`](#fn-specforproviderfeaturetagswithcustomsinglesignon)
      * [`fn withEnterprise(enterprise)`](#fn-specforproviderfeaturetagswithenterprise)
      * [`fn withGallery(gallery)`](#fn-specforproviderfeaturetagswithgallery)
      * [`fn withHide(hide)`](#fn-specforproviderfeaturetagswithhide)
    * [`obj spec.forProvider.samlSingleSignOn`](#obj-specforprovidersamlsinglesignon)
      * [`fn withRelayState(relayState)`](#fn-specforprovidersamlsinglesignonwithrelaystate)
  * [`obj spec.initProvider`](#obj-specinitprovider)
    * [`fn withAccountEnabled(accountEnabled)`](#fn-specinitproviderwithaccountenabled)
    * [`fn withAlternativeNames(alternativeNames)`](#fn-specinitproviderwithalternativenames)
    * [`fn withAlternativeNamesMixin(alternativeNames)`](#fn-specinitproviderwithalternativenamesmixin)
    * [`fn withAppRoleAssignmentRequired(appRoleAssignmentRequired)`](#fn-specinitproviderwithapproleassignmentrequired)
    * [`fn withClientId(clientId)`](#fn-specinitproviderwithclientid)
    * [`fn withDescription(description)`](#fn-specinitproviderwithdescription)
    * [`fn withFeatureTags(featureTags)`](#fn-specinitproviderwithfeaturetags)
    * [`fn withFeatureTagsMixin(featureTags)`](#fn-specinitproviderwithfeaturetagsmixin)
    * [`fn withLoginUrl(loginUrl)`](#fn-specinitproviderwithloginurl)
    * [`fn withNotes(notes)`](#fn-specinitproviderwithnotes)
    * [`fn withNotificationEmailAddresses(notificationEmailAddresses)`](#fn-specinitproviderwithnotificationemailaddresses)
    * [`fn withNotificationEmailAddressesMixin(notificationEmailAddresses)`](#fn-specinitproviderwithnotificationemailaddressesmixin)
    * [`fn withOwners(owners)`](#fn-specinitproviderwithowners)
    * [`fn withOwnersMixin(owners)`](#fn-specinitproviderwithownersmixin)
    * [`fn withPreferredSingleSignOnMode(preferredSingleSignOnMode)`](#fn-specinitproviderwithpreferredsinglesignonmode)
    * [`fn withSamlSingleSignOn(samlSingleSignOn)`](#fn-specinitproviderwithsamlsinglesignon)
    * [`fn withSamlSingleSignOnMixin(samlSingleSignOn)`](#fn-specinitproviderwithsamlsinglesignonmixin)
    * [`fn withTags(tags)`](#fn-specinitproviderwithtags)
    * [`fn withTagsMixin(tags)`](#fn-specinitproviderwithtagsmixin)
    * [`fn withUseExisting(useExisting)`](#fn-specinitproviderwithuseexisting)
    * [`obj spec.initProvider.clientIdRef`](#obj-specinitproviderclientidref)
      * [`fn withName(name)`](#fn-specinitproviderclientidrefwithname)
      * [`obj spec.initProvider.clientIdRef.policy`](#obj-specinitproviderclientidrefpolicy)
        * [`fn withResolution(resolution)`](#fn-specinitproviderclientidrefpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specinitproviderclientidrefpolicywithresolve)
    * [`obj spec.initProvider.clientIdSelector`](#obj-specinitproviderclientidselector)
      * [`fn withMatchControllerRef(matchControllerRef)`](#fn-specinitproviderclientidselectorwithmatchcontrollerref)
      * [`fn withMatchLabels(matchLabels)`](#fn-specinitproviderclientidselectorwithmatchlabels)
      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specinitproviderclientidselectorwithmatchlabelsmixin)
      * [`obj spec.initProvider.clientIdSelector.policy`](#obj-specinitproviderclientidselectorpolicy)
        * [`fn withResolution(resolution)`](#fn-specinitproviderclientidselectorpolicywithresolution)
        * [`fn withResolve(resolve)`](#fn-specinitproviderclientidselectorpolicywithresolve)
    * [`obj spec.initProvider.featureTags`](#obj-specinitproviderfeaturetags)
      * [`fn withCustomSingleSignOn(customSingleSignOn)`](#fn-specinitproviderfeaturetagswithcustomsinglesignon)
      * [`fn withEnterprise(enterprise)`](#fn-specinitproviderfeaturetagswithenterprise)
      * [`fn withGallery(gallery)`](#fn-specinitproviderfeaturetagswithgallery)
      * [`fn withHide(hide)`](#fn-specinitproviderfeaturetagswithhide)
    * [`obj spec.initProvider.samlSingleSignOn`](#obj-specinitprovidersamlsinglesignon)
      * [`fn withRelayState(relayState)`](#fn-specinitprovidersamlsinglesignonwithrelaystate)
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

new returns an instance of Principal

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

"PrincipalSpec defines the desired state of Principal"

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



### fn spec.forProvider.withAccountEnabled

```ts
withAccountEnabled(accountEnabled)
```

"Whether or not the service principal account is enabled. Defaults to true.\nWhether or not the service principal account is enabled"

### fn spec.forProvider.withAlternativeNames

```ts
withAlternativeNames(alternativeNames)
```

"A set of alternative names, used to retrieve service principals by subscription, identify resource group and full resource ids for managed identities.\nA list of alternative names, used to retrieve service principals by subscription, identify resource group and full resource ids for managed identities"

### fn spec.forProvider.withAlternativeNamesMixin

```ts
withAlternativeNamesMixin(alternativeNames)
```

"A set of alternative names, used to retrieve service principals by subscription, identify resource group and full resource ids for managed identities.\nA list of alternative names, used to retrieve service principals by subscription, identify resource group and full resource ids for managed identities"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withAppRoleAssignmentRequired

```ts
withAppRoleAssignmentRequired(appRoleAssignmentRequired)
```

"Whether this service principal requires an app role assignment to a user or group before Azure AD will issue a user or access token to the application. Defaults to false.\nWhether this service principal requires an app role assignment to a user or group before Azure AD will issue a user or access token to the application"

### fn spec.forProvider.withClientId

```ts
withClientId(clientId)
```

"The client ID of the application for which to create a service principal.\nThe client ID of the application for which to create a service principal"

### fn spec.forProvider.withDescription

```ts
withDescription(description)
```

"A description of the service principal provided for internal end-users.\nDescription of the service principal provided for internal end-users"

### fn spec.forProvider.withFeatureTags

```ts
withFeatureTags(featureTags)
```

"A feature_tags block as described below. Cannot be used together with the tags property.\nBlock of features to configure for this service principal using tags"

### fn spec.forProvider.withFeatureTagsMixin

```ts
withFeatureTagsMixin(featureTags)
```

"A feature_tags block as described below. Cannot be used together with the tags property.\nBlock of features to configure for this service principal using tags"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withLoginUrl

```ts
withLoginUrl(loginUrl)
```

"The URL where the service provider redirects the user to Azure AD to authenticate. Azure AD uses the URL to launch the application from Microsoft 365 or the Azure AD My Apps. When blank, Azure AD performs IdP-initiated sign-on for applications configured with SAML-based single sign-on.\nThe URL where the service provider redirects the user to Azure AD to authenticate. Azure AD uses the URL to launch the application from Microsoft 365 or the Azure AD My Apps. When blank, Azure AD performs IdP-initiated sign-on for applications configured with SAML-based single sign-on"

### fn spec.forProvider.withNotes

```ts
withNotes(notes)
```

"A free text field to capture information about the service principal, typically used for operational purposes.\nFree text field to capture information about the service principal, typically used for operational purposes"

### fn spec.forProvider.withNotificationEmailAddresses

```ts
withNotificationEmailAddresses(notificationEmailAddresses)
```

"A set of email addresses where Azure AD sends a notification when the active certificate is near the expiration date. This is only for the certificates used to sign the SAML token issued for Azure AD Gallery applications.\nList of email addresses where Azure AD sends a notification when the active certificate is near the expiration date. This is only for the certificates used to sign the SAML token issued for Azure AD Gallery applications"

### fn spec.forProvider.withNotificationEmailAddressesMixin

```ts
withNotificationEmailAddressesMixin(notificationEmailAddresses)
```

"A set of email addresses where Azure AD sends a notification when the active certificate is near the expiration date. This is only for the certificates used to sign the SAML token issued for Azure AD Gallery applications.\nList of email addresses where Azure AD sends a notification when the active certificate is near the expiration date. This is only for the certificates used to sign the SAML token issued for Azure AD Gallery applications"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withOwners

```ts
withOwners(owners)
```

"A set of object IDs of principals that will be granted ownership of the service principal. Supported object types are users or service principals. By default, no owners are assigned.\nA list of object IDs of principals that will be granted ownership of the service principal"

### fn spec.forProvider.withOwnersMixin

```ts
withOwnersMixin(owners)
```

"A set of object IDs of principals that will be granted ownership of the service principal. Supported object types are users or service principals. By default, no owners are assigned.\nA list of object IDs of principals that will be granted ownership of the service principal"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withPreferredSingleSignOnMode

```ts
withPreferredSingleSignOnMode(preferredSingleSignOnMode)
```

"The single sign-on mode configured for this application. Azure AD uses the preferred single sign-on mode to launch the application from Microsoft 365 or the Azure AD My Apps. Supported values are oidc, password, saml or notSupported. Omit this property or specify a blank string to unset.\nThe single sign-on mode configured for this application. Azure AD uses the preferred single sign-on mode to launch the application from Microsoft 365 or the Azure AD My Apps"

### fn spec.forProvider.withSamlSingleSignOn

```ts
withSamlSingleSignOn(samlSingleSignOn)
```

"A saml_single_sign_on block as documented below.\nSettings related to SAML single sign-on"

### fn spec.forProvider.withSamlSingleSignOnMixin

```ts
withSamlSingleSignOnMixin(samlSingleSignOn)
```

"A saml_single_sign_on block as documented below.\nSettings related to SAML single sign-on"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withTags

```ts
withTags(tags)
```

"A set of tags to apply to the service principal for configuring specific behaviours of the service principal. Note that these are not provided for use by practitioners. Cannot be used together with the feature_tags block.\nA set of tags to apply to the service principal"

### fn spec.forProvider.withTagsMixin

```ts
withTagsMixin(tags)
```

"A set of tags to apply to the service principal for configuring specific behaviours of the service principal. Note that these are not provided for use by practitioners. Cannot be used together with the feature_tags block.\nA set of tags to apply to the service principal"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withUseExisting

```ts
withUseExisting(useExisting)
```

"When true, any existing service principal linked to the same application will be automatically imported. When false, an import error will be raised for any pre-existing service principal.\nWhen true, the resource will return an existing service principal instead of failing with an error"

## obj spec.forProvider.clientIdRef

"Reference to a Application in applications to populate clientId."

### fn spec.forProvider.clientIdRef.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.forProvider.clientIdRef.policy

"Policies for referencing."

### fn spec.forProvider.clientIdRef.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.forProvider.clientIdRef.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.forProvider.clientIdSelector

"Selector for a Application in applications to populate clientId."

### fn spec.forProvider.clientIdSelector.withMatchControllerRef

```ts
withMatchControllerRef(matchControllerRef)
```

"MatchControllerRef ensures an object with the same controller reference\nas the selecting object is selected."

### fn spec.forProvider.clientIdSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

### fn spec.forProvider.clientIdSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.clientIdSelector.policy

"Policies for selection."

### fn spec.forProvider.clientIdSelector.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.forProvider.clientIdSelector.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.forProvider.featureTags

"A feature_tags block as described below. Cannot be used together with the tags property.\nBlock of features to configure for this service principal using tags"

### fn spec.forProvider.featureTags.withCustomSingleSignOn

```ts
withCustomSingleSignOn(customSingleSignOn)
```

"Whether this service principal represents a custom SAML application. Enabling this will assign the WindowsAzureActiveDirectoryCustomSingleSignOnApplication tag. Defaults to false.\nWhether this service principal represents a custom SAML application"

### fn spec.forProvider.featureTags.withEnterprise

```ts
withEnterprise(enterprise)
```

"Whether this service principal represents an Enterprise Application. Enabling this will assign the WindowsAzureActiveDirectoryIntegratedApp tag. Defaults to false.\nWhether this service principal represents an Enterprise Application"

### fn spec.forProvider.featureTags.withGallery

```ts
withGallery(gallery)
```

"Whether this service principal represents a gallery application. Enabling this will assign the WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1 tag. Defaults to false.\nWhether this service principal represents a gallery application"

### fn spec.forProvider.featureTags.withHide

```ts
withHide(hide)
```

"Whether this app is invisible to users in My Apps and Office 365 Launcher. Enabling this will assign the HideApp tag. Defaults to false.\nWhether this app is invisible to users in My Apps and Office 365 Launcher"

## obj spec.forProvider.samlSingleSignOn

"A saml_single_sign_on block as documented below.\nSettings related to SAML single sign-on"

### fn spec.forProvider.samlSingleSignOn.withRelayState

```ts
withRelayState(relayState)
```

"The relative URI the service provider would redirect to after completion of the single sign-on flow.\nThe relative URI the service provider would redirect to after completion of the single sign-on flow"

## obj spec.initProvider

"THIS IS A BETA FIELD. It will be honored\nunless the Management Policies feature flag is disabled.\nInitProvider holds the same fields as ForProvider, with the exception\nof Identifier and other resource reference fields. The fields that are\nin InitProvider are merged into ForProvider when the resource is created.\nThe same fields are also added to the terraform ignore_changes hook, to\navoid updating them after creation. This is useful for fields that are\nrequired on creation, but we do not desire to update them after creation,\nfor example because of an external controller is managing them, like an\nautoscaler."

### fn spec.initProvider.withAccountEnabled

```ts
withAccountEnabled(accountEnabled)
```

"Whether or not the service principal account is enabled. Defaults to true.\nWhether or not the service principal account is enabled"

### fn spec.initProvider.withAlternativeNames

```ts
withAlternativeNames(alternativeNames)
```

"A set of alternative names, used to retrieve service principals by subscription, identify resource group and full resource ids for managed identities.\nA list of alternative names, used to retrieve service principals by subscription, identify resource group and full resource ids for managed identities"

### fn spec.initProvider.withAlternativeNamesMixin

```ts
withAlternativeNamesMixin(alternativeNames)
```

"A set of alternative names, used to retrieve service principals by subscription, identify resource group and full resource ids for managed identities.\nA list of alternative names, used to retrieve service principals by subscription, identify resource group and full resource ids for managed identities"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withAppRoleAssignmentRequired

```ts
withAppRoleAssignmentRequired(appRoleAssignmentRequired)
```

"Whether this service principal requires an app role assignment to a user or group before Azure AD will issue a user or access token to the application. Defaults to false.\nWhether this service principal requires an app role assignment to a user or group before Azure AD will issue a user or access token to the application"

### fn spec.initProvider.withClientId

```ts
withClientId(clientId)
```

"The client ID of the application for which to create a service principal.\nThe client ID of the application for which to create a service principal"

### fn spec.initProvider.withDescription

```ts
withDescription(description)
```

"A description of the service principal provided for internal end-users.\nDescription of the service principal provided for internal end-users"

### fn spec.initProvider.withFeatureTags

```ts
withFeatureTags(featureTags)
```

"A feature_tags block as described below. Cannot be used together with the tags property.\nBlock of features to configure for this service principal using tags"

### fn spec.initProvider.withFeatureTagsMixin

```ts
withFeatureTagsMixin(featureTags)
```

"A feature_tags block as described below. Cannot be used together with the tags property.\nBlock of features to configure for this service principal using tags"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withLoginUrl

```ts
withLoginUrl(loginUrl)
```

"The URL where the service provider redirects the user to Azure AD to authenticate. Azure AD uses the URL to launch the application from Microsoft 365 or the Azure AD My Apps. When blank, Azure AD performs IdP-initiated sign-on for applications configured with SAML-based single sign-on.\nThe URL where the service provider redirects the user to Azure AD to authenticate. Azure AD uses the URL to launch the application from Microsoft 365 or the Azure AD My Apps. When blank, Azure AD performs IdP-initiated sign-on for applications configured with SAML-based single sign-on"

### fn spec.initProvider.withNotes

```ts
withNotes(notes)
```

"A free text field to capture information about the service principal, typically used for operational purposes.\nFree text field to capture information about the service principal, typically used for operational purposes"

### fn spec.initProvider.withNotificationEmailAddresses

```ts
withNotificationEmailAddresses(notificationEmailAddresses)
```

"A set of email addresses where Azure AD sends a notification when the active certificate is near the expiration date. This is only for the certificates used to sign the SAML token issued for Azure AD Gallery applications.\nList of email addresses where Azure AD sends a notification when the active certificate is near the expiration date. This is only for the certificates used to sign the SAML token issued for Azure AD Gallery applications"

### fn spec.initProvider.withNotificationEmailAddressesMixin

```ts
withNotificationEmailAddressesMixin(notificationEmailAddresses)
```

"A set of email addresses where Azure AD sends a notification when the active certificate is near the expiration date. This is only for the certificates used to sign the SAML token issued for Azure AD Gallery applications.\nList of email addresses where Azure AD sends a notification when the active certificate is near the expiration date. This is only for the certificates used to sign the SAML token issued for Azure AD Gallery applications"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withOwners

```ts
withOwners(owners)
```

"A set of object IDs of principals that will be granted ownership of the service principal. Supported object types are users or service principals. By default, no owners are assigned.\nA list of object IDs of principals that will be granted ownership of the service principal"

### fn spec.initProvider.withOwnersMixin

```ts
withOwnersMixin(owners)
```

"A set of object IDs of principals that will be granted ownership of the service principal. Supported object types are users or service principals. By default, no owners are assigned.\nA list of object IDs of principals that will be granted ownership of the service principal"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withPreferredSingleSignOnMode

```ts
withPreferredSingleSignOnMode(preferredSingleSignOnMode)
```

"The single sign-on mode configured for this application. Azure AD uses the preferred single sign-on mode to launch the application from Microsoft 365 or the Azure AD My Apps. Supported values are oidc, password, saml or notSupported. Omit this property or specify a blank string to unset.\nThe single sign-on mode configured for this application. Azure AD uses the preferred single sign-on mode to launch the application from Microsoft 365 or the Azure AD My Apps"

### fn spec.initProvider.withSamlSingleSignOn

```ts
withSamlSingleSignOn(samlSingleSignOn)
```

"A saml_single_sign_on block as documented below.\nSettings related to SAML single sign-on"

### fn spec.initProvider.withSamlSingleSignOnMixin

```ts
withSamlSingleSignOnMixin(samlSingleSignOn)
```

"A saml_single_sign_on block as documented below.\nSettings related to SAML single sign-on"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withTags

```ts
withTags(tags)
```

"A set of tags to apply to the service principal for configuring specific behaviours of the service principal. Note that these are not provided for use by practitioners. Cannot be used together with the feature_tags block.\nA set of tags to apply to the service principal"

### fn spec.initProvider.withTagsMixin

```ts
withTagsMixin(tags)
```

"A set of tags to apply to the service principal for configuring specific behaviours of the service principal. Note that these are not provided for use by practitioners. Cannot be used together with the feature_tags block.\nA set of tags to apply to the service principal"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withUseExisting

```ts
withUseExisting(useExisting)
```

"When true, any existing service principal linked to the same application will be automatically imported. When false, an import error will be raised for any pre-existing service principal.\nWhen true, the resource will return an existing service principal instead of failing with an error"

## obj spec.initProvider.clientIdRef

"Reference to a Application in applications to populate clientId."

### fn spec.initProvider.clientIdRef.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.initProvider.clientIdRef.policy

"Policies for referencing."

### fn spec.initProvider.clientIdRef.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.initProvider.clientIdRef.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.initProvider.clientIdSelector

"Selector for a Application in applications to populate clientId."

### fn spec.initProvider.clientIdSelector.withMatchControllerRef

```ts
withMatchControllerRef(matchControllerRef)
```

"MatchControllerRef ensures an object with the same controller reference\nas the selecting object is selected."

### fn spec.initProvider.clientIdSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

### fn spec.initProvider.clientIdSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.clientIdSelector.policy

"Policies for selection."

### fn spec.initProvider.clientIdSelector.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.initProvider.clientIdSelector.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.initProvider.featureTags

"A feature_tags block as described below. Cannot be used together with the tags property.\nBlock of features to configure for this service principal using tags"

### fn spec.initProvider.featureTags.withCustomSingleSignOn

```ts
withCustomSingleSignOn(customSingleSignOn)
```

"Whether this service principal represents a custom SAML application. Enabling this will assign the WindowsAzureActiveDirectoryCustomSingleSignOnApplication tag. Defaults to false.\nWhether this service principal represents a custom SAML application"

### fn spec.initProvider.featureTags.withEnterprise

```ts
withEnterprise(enterprise)
```

"Whether this service principal represents an Enterprise Application. Enabling this will assign the WindowsAzureActiveDirectoryIntegratedApp tag. Defaults to false.\nWhether this service principal represents an Enterprise Application"

### fn spec.initProvider.featureTags.withGallery

```ts
withGallery(gallery)
```

"Whether this service principal represents a gallery application. Enabling this will assign the WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1 tag. Defaults to false.\nWhether this service principal represents a gallery application"

### fn spec.initProvider.featureTags.withHide

```ts
withHide(hide)
```

"Whether this app is invisible to users in My Apps and Office 365 Launcher. Enabling this will assign the HideApp tag. Defaults to false.\nWhether this app is invisible to users in My Apps and Office 365 Launcher"

## obj spec.initProvider.samlSingleSignOn

"A saml_single_sign_on block as documented below.\nSettings related to SAML single sign-on"

### fn spec.initProvider.samlSingleSignOn.withRelayState

```ts
withRelayState(relayState)
```

"The relative URI the service provider would redirect to after completion of the single sign-on flow.\nThe relative URI the service provider would redirect to after completion of the single sign-on flow"

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