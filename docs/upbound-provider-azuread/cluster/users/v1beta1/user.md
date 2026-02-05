---
permalink: /upbound-provider-azuread/cluster/users/v1beta1/user/
---

# users.v1beta1.user

"User is the Schema for the Users API."

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
    * [`fn withAgeGroup(ageGroup)`](#fn-specforproviderwithagegroup)
    * [`fn withBusinessPhones(businessPhones)`](#fn-specforproviderwithbusinessphones)
    * [`fn withBusinessPhonesMixin(businessPhones)`](#fn-specforproviderwithbusinessphonesmixin)
    * [`fn withCity(city)`](#fn-specforproviderwithcity)
    * [`fn withCompanyName(companyName)`](#fn-specforproviderwithcompanyname)
    * [`fn withConsentProvidedForMinor(consentProvidedForMinor)`](#fn-specforproviderwithconsentprovidedforminor)
    * [`fn withCostCenter(costCenter)`](#fn-specforproviderwithcostcenter)
    * [`fn withCountry(country)`](#fn-specforproviderwithcountry)
    * [`fn withDepartment(department)`](#fn-specforproviderwithdepartment)
    * [`fn withDisablePasswordExpiration(disablePasswordExpiration)`](#fn-specforproviderwithdisablepasswordexpiration)
    * [`fn withDisableStrongPassword(disableStrongPassword)`](#fn-specforproviderwithdisablestrongpassword)
    * [`fn withDisplayName(displayName)`](#fn-specforproviderwithdisplayname)
    * [`fn withDivision(division)`](#fn-specforproviderwithdivision)
    * [`fn withEmployeeHireDate(employeeHireDate)`](#fn-specforproviderwithemployeehiredate)
    * [`fn withEmployeeId(employeeId)`](#fn-specforproviderwithemployeeid)
    * [`fn withEmployeeType(employeeType)`](#fn-specforproviderwithemployeetype)
    * [`fn withFaxNumber(faxNumber)`](#fn-specforproviderwithfaxnumber)
    * [`fn withForcePasswordChange(forcePasswordChange)`](#fn-specforproviderwithforcepasswordchange)
    * [`fn withGivenName(givenName)`](#fn-specforproviderwithgivenname)
    * [`fn withJobTitle(jobTitle)`](#fn-specforproviderwithjobtitle)
    * [`fn withMail(mail)`](#fn-specforproviderwithmail)
    * [`fn withMailNickname(mailNickname)`](#fn-specforproviderwithmailnickname)
    * [`fn withManagerId(managerId)`](#fn-specforproviderwithmanagerid)
    * [`fn withMobilePhone(mobilePhone)`](#fn-specforproviderwithmobilephone)
    * [`fn withOfficeLocation(officeLocation)`](#fn-specforproviderwithofficelocation)
    * [`fn withOnpremisesImmutableId(onpremisesImmutableId)`](#fn-specforproviderwithonpremisesimmutableid)
    * [`fn withOtherMails(otherMails)`](#fn-specforproviderwithothermails)
    * [`fn withOtherMailsMixin(otherMails)`](#fn-specforproviderwithothermailsmixin)
    * [`fn withPostalCode(postalCode)`](#fn-specforproviderwithpostalcode)
    * [`fn withPreferredLanguage(preferredLanguage)`](#fn-specforproviderwithpreferredlanguage)
    * [`fn withShowInAddressList(showInAddressList)`](#fn-specforproviderwithshowinaddresslist)
    * [`fn withState(state)`](#fn-specforproviderwithstate)
    * [`fn withStreetAddress(streetAddress)`](#fn-specforproviderwithstreetaddress)
    * [`fn withSurname(surname)`](#fn-specforproviderwithsurname)
    * [`fn withUsageLocation(usageLocation)`](#fn-specforproviderwithusagelocation)
    * [`fn withUserPrincipalName(userPrincipalName)`](#fn-specforproviderwithuserprincipalname)
    * [`obj spec.forProvider.passwordSecretRef`](#obj-specforproviderpasswordsecretref)
      * [`fn withKey(key)`](#fn-specforproviderpasswordsecretrefwithkey)
      * [`fn withName(name)`](#fn-specforproviderpasswordsecretrefwithname)
      * [`fn withNamespace(namespace)`](#fn-specforproviderpasswordsecretrefwithnamespace)
  * [`obj spec.initProvider`](#obj-specinitprovider)
    * [`fn withAccountEnabled(accountEnabled)`](#fn-specinitproviderwithaccountenabled)
    * [`fn withAgeGroup(ageGroup)`](#fn-specinitproviderwithagegroup)
    * [`fn withBusinessPhones(businessPhones)`](#fn-specinitproviderwithbusinessphones)
    * [`fn withBusinessPhonesMixin(businessPhones)`](#fn-specinitproviderwithbusinessphonesmixin)
    * [`fn withCity(city)`](#fn-specinitproviderwithcity)
    * [`fn withCompanyName(companyName)`](#fn-specinitproviderwithcompanyname)
    * [`fn withConsentProvidedForMinor(consentProvidedForMinor)`](#fn-specinitproviderwithconsentprovidedforminor)
    * [`fn withCostCenter(costCenter)`](#fn-specinitproviderwithcostcenter)
    * [`fn withCountry(country)`](#fn-specinitproviderwithcountry)
    * [`fn withDepartment(department)`](#fn-specinitproviderwithdepartment)
    * [`fn withDisablePasswordExpiration(disablePasswordExpiration)`](#fn-specinitproviderwithdisablepasswordexpiration)
    * [`fn withDisableStrongPassword(disableStrongPassword)`](#fn-specinitproviderwithdisablestrongpassword)
    * [`fn withDisplayName(displayName)`](#fn-specinitproviderwithdisplayname)
    * [`fn withDivision(division)`](#fn-specinitproviderwithdivision)
    * [`fn withEmployeeHireDate(employeeHireDate)`](#fn-specinitproviderwithemployeehiredate)
    * [`fn withEmployeeId(employeeId)`](#fn-specinitproviderwithemployeeid)
    * [`fn withEmployeeType(employeeType)`](#fn-specinitproviderwithemployeetype)
    * [`fn withFaxNumber(faxNumber)`](#fn-specinitproviderwithfaxnumber)
    * [`fn withForcePasswordChange(forcePasswordChange)`](#fn-specinitproviderwithforcepasswordchange)
    * [`fn withGivenName(givenName)`](#fn-specinitproviderwithgivenname)
    * [`fn withJobTitle(jobTitle)`](#fn-specinitproviderwithjobtitle)
    * [`fn withMail(mail)`](#fn-specinitproviderwithmail)
    * [`fn withMailNickname(mailNickname)`](#fn-specinitproviderwithmailnickname)
    * [`fn withManagerId(managerId)`](#fn-specinitproviderwithmanagerid)
    * [`fn withMobilePhone(mobilePhone)`](#fn-specinitproviderwithmobilephone)
    * [`fn withOfficeLocation(officeLocation)`](#fn-specinitproviderwithofficelocation)
    * [`fn withOnpremisesImmutableId(onpremisesImmutableId)`](#fn-specinitproviderwithonpremisesimmutableid)
    * [`fn withOtherMails(otherMails)`](#fn-specinitproviderwithothermails)
    * [`fn withOtherMailsMixin(otherMails)`](#fn-specinitproviderwithothermailsmixin)
    * [`fn withPostalCode(postalCode)`](#fn-specinitproviderwithpostalcode)
    * [`fn withPreferredLanguage(preferredLanguage)`](#fn-specinitproviderwithpreferredlanguage)
    * [`fn withShowInAddressList(showInAddressList)`](#fn-specinitproviderwithshowinaddresslist)
    * [`fn withState(state)`](#fn-specinitproviderwithstate)
    * [`fn withStreetAddress(streetAddress)`](#fn-specinitproviderwithstreetaddress)
    * [`fn withSurname(surname)`](#fn-specinitproviderwithsurname)
    * [`fn withUsageLocation(usageLocation)`](#fn-specinitproviderwithusagelocation)
    * [`fn withUserPrincipalName(userPrincipalName)`](#fn-specinitproviderwithuserprincipalname)
    * [`obj spec.initProvider.passwordSecretRef`](#obj-specinitproviderpasswordsecretref)
      * [`fn withKey(key)`](#fn-specinitproviderpasswordsecretrefwithkey)
      * [`fn withName(name)`](#fn-specinitproviderpasswordsecretrefwithname)
      * [`fn withNamespace(namespace)`](#fn-specinitproviderpasswordsecretrefwithnamespace)
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

new returns an instance of User

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

"UserSpec defines the desired state of User"

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

"Whether or not the account should be enabled.\nWhether or not the account should be enabled"

### fn spec.forProvider.withAgeGroup

```ts
withAgeGroup(ageGroup)
```

"The age group of the user. Supported values are Adult, NotAdult and Minor. Omit this property or specify a blank string to unset.\nThe age group of the user"

### fn spec.forProvider.withBusinessPhones

```ts
withBusinessPhones(businessPhones)
```

"A list of telephone numbers for the user. Only one number can be set for this property. Read-only for users synced with Azure AD Connect.\nThe telephone numbers for the user. Only one number can be set for this property. Read-only for users synced with Azure AD Connect"

### fn spec.forProvider.withBusinessPhonesMixin

```ts
withBusinessPhonesMixin(businessPhones)
```

"A list of telephone numbers for the user. Only one number can be set for this property. Read-only for users synced with Azure AD Connect.\nThe telephone numbers for the user. Only one number can be set for this property. Read-only for users synced with Azure AD Connect"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withCity

```ts
withCity(city)
```

"The city in which the user is located.\nThe city in which the user is located"

### fn spec.forProvider.withCompanyName

```ts
withCompanyName(companyName)
```

"The company name which the user is associated. This property can be useful for describing the company that an external user comes from.\nThe company name which the user is associated. This property can be useful for describing the company that an external user comes from"

### fn spec.forProvider.withConsentProvidedForMinor

```ts
withConsentProvidedForMinor(consentProvidedForMinor)
```

"Whether consent has been obtained for minors. Supported values are Granted, Denied and NotRequired. Omit this property or specify a blank string to unset.\nWhether consent has been obtained for minors"

### fn spec.forProvider.withCostCenter

```ts
withCostCenter(costCenter)
```

"The cost center associated with the user.\nThe cost center associated with the user."

### fn spec.forProvider.withCountry

```ts
withCountry(country)
```

"The country/region in which the user is located. Examples include: NO, JP, and GB.\nThe country/region in which the user is located, e.g. `US` or `UK`"

### fn spec.forProvider.withDepartment

```ts
withDepartment(department)
```

"The name for the department in which the user works.\nThe name for the department in which the user works"

### fn spec.forProvider.withDisablePasswordExpiration

```ts
withDisablePasswordExpiration(disablePasswordExpiration)
```

"Whether the user's password is exempt from expiring. Defaults to false.\nWhether the users password is exempt from expiring"

### fn spec.forProvider.withDisableStrongPassword

```ts
withDisableStrongPassword(disableStrongPassword)
```

"Whether the user is allowed weaker passwords than the default policy to be specified. Defaults to false.\nWhether the user is allowed weaker passwords than the default policy to be specified."

### fn spec.forProvider.withDisplayName

```ts
withDisplayName(displayName)
```

"The name to display in the address book for the user.\nThe name to display in the address book for the user"

### fn spec.forProvider.withDivision

```ts
withDivision(division)
```

"The name of the division in which the user works.\nThe name of the division in which the user works."

### fn spec.forProvider.withEmployeeHireDate

```ts
withEmployeeHireDate(employeeHireDate)
```

"The hire date of the user, formatted as an RFC3339 date string (e.g. 2018-01-01T01:02:03Z).\nThe hire date of the user, formatted as an RFC3339 date string (e.g. `2018-01-01T01:02:03Z`)."

### fn spec.forProvider.withEmployeeId

```ts
withEmployeeId(employeeId)
```

"The employee identifier assigned to the user by the organisation.\nThe employee identifier assigned to the user by the organisation"

### fn spec.forProvider.withEmployeeType

```ts
withEmployeeType(employeeType)
```

"Captures enterprise worker type. For example, Employee, Contractor, Consultant, or Vendor.\nCaptures enterprise worker type. For example, Employee, Contractor, Consultant, or Vendor."

### fn spec.forProvider.withFaxNumber

```ts
withFaxNumber(faxNumber)
```

"The fax number of the user.\nThe fax number of the user"

### fn spec.forProvider.withForcePasswordChange

```ts
withForcePasswordChange(forcePasswordChange)
```

"Whether the user is forced to change the password during the next sign-in. Only takes effect when also changing the password. Defaults to false.\nWhether the user is forced to change the password during the next sign-in. Only takes effect when also changing the password"

### fn spec.forProvider.withGivenName

```ts
withGivenName(givenName)
```

"The given name (first name) of the user.\nThe given name (first name) of the user"

### fn spec.forProvider.withJobTitle

```ts
withJobTitle(jobTitle)
```

"The user’s job title.\nThe user’s job title"

### fn spec.forProvider.withMail

```ts
withMail(mail)
```

"The SMTP address for the user. This property cannot be unset once specified.\nThe SMTP address for the user. Cannot be unset."

### fn spec.forProvider.withMailNickname

```ts
withMailNickname(mailNickname)
```

"The mail alias for the user. Defaults to the user name part of the user principal name (UPN).\nThe mail alias for the user. Defaults to the user name part of the user principal name (UPN)"

### fn spec.forProvider.withManagerId

```ts
withManagerId(managerId)
```

"The object ID of the user's manager.\nThe object ID of the user's manager"

### fn spec.forProvider.withMobilePhone

```ts
withMobilePhone(mobilePhone)
```

"The primary cellular telephone number for the user.\nThe primary cellular telephone number for the user"

### fn spec.forProvider.withOfficeLocation

```ts
withOfficeLocation(officeLocation)
```

"The office location in the user's place of business.\nThe office location in the user's place of business"

### fn spec.forProvider.withOnpremisesImmutableId

```ts
withOnpremisesImmutableId(onpremisesImmutableId)
```

"The value used to associate an on-premise Active Directory user account with their Azure AD user object. This must be specified if you are using a federated domain for the user's user_principal_name property when creating a new user account.\nThe value used to associate an on-premise Active Directory user account with their Azure AD user object. This must be specified if you are using a federated domain for the user's `user_principal_name` property when creating a new user account"

### fn spec.forProvider.withOtherMails

```ts
withOtherMails(otherMails)
```

"A list of additional email addresses for the user.\nAdditional email addresses for the user"

### fn spec.forProvider.withOtherMailsMixin

```ts
withOtherMailsMixin(otherMails)
```

"A list of additional email addresses for the user.\nAdditional email addresses for the user"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withPostalCode

```ts
withPostalCode(postalCode)
```

"The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.\nThe postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code"

### fn spec.forProvider.withPreferredLanguage

```ts
withPreferredLanguage(preferredLanguage)
```

"The user's preferred language, in ISO 639-1 notation.\nThe user's preferred language, in ISO 639-1 notation"

### fn spec.forProvider.withShowInAddressList

```ts
withShowInAddressList(showInAddressList)
```

"Whether or not the Outlook global address list should include this user. Defaults to true.\nWhether or not the Outlook global address list should include this user"

### fn spec.forProvider.withState

```ts
withState(state)
```

"The state or province in the user's address.\nThe state or province in the user's address"

### fn spec.forProvider.withStreetAddress

```ts
withStreetAddress(streetAddress)
```

"The street address of the user's place of business.\nThe street address of the user's place of business"

### fn spec.forProvider.withSurname

```ts
withSurname(surname)
```

"The user's surname (family name or last name).\nThe user's surname (family name or last name)"

### fn spec.forProvider.withUsageLocation

```ts
withUsageLocation(usageLocation)
```

"The usage location of the user. Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries. The usage location is a two letter country code (ISO standard 3166). Examples include: NO, JP, and GB. Cannot be reset to null once set.\nThe usage location of the user. Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries. The usage location is a two letter country code (ISO standard 3166). Examples include: `NO`, `JP`, and `GB`. Cannot be reset to null once set"

### fn spec.forProvider.withUserPrincipalName

```ts
withUserPrincipalName(userPrincipalName)
```

"The user principal name (UPN) of the user.\nThe user principal name (UPN) of the user"

## obj spec.forProvider.passwordSecretRef

"The password for the user. The password must satisfy minimum requirements as specified by the password policy. The maximum length is 256 characters. This property is required when creating a new user.\nThe password for the user. The password must satisfy minimum requirements as specified by the password policy. The maximum length is 256 characters. This property is required when creating a new user"

### fn spec.forProvider.passwordSecretRef.withKey

```ts
withKey(key)
```

"The key to select."

### fn spec.forProvider.passwordSecretRef.withName

```ts
withName(name)
```

"Name of the secret."

### fn spec.forProvider.passwordSecretRef.withNamespace

```ts
withNamespace(namespace)
```

"Namespace of the secret."

## obj spec.initProvider

"THIS IS A BETA FIELD. It will be honored\nunless the Management Policies feature flag is disabled.\nInitProvider holds the same fields as ForProvider, with the exception\nof Identifier and other resource reference fields. The fields that are\nin InitProvider are merged into ForProvider when the resource is created.\nThe same fields are also added to the terraform ignore_changes hook, to\navoid updating them after creation. This is useful for fields that are\nrequired on creation, but we do not desire to update them after creation,\nfor example because of an external controller is managing them, like an\nautoscaler."

### fn spec.initProvider.withAccountEnabled

```ts
withAccountEnabled(accountEnabled)
```

"Whether or not the account should be enabled.\nWhether or not the account should be enabled"

### fn spec.initProvider.withAgeGroup

```ts
withAgeGroup(ageGroup)
```

"The age group of the user. Supported values are Adult, NotAdult and Minor. Omit this property or specify a blank string to unset.\nThe age group of the user"

### fn spec.initProvider.withBusinessPhones

```ts
withBusinessPhones(businessPhones)
```

"A list of telephone numbers for the user. Only one number can be set for this property. Read-only for users synced with Azure AD Connect.\nThe telephone numbers for the user. Only one number can be set for this property. Read-only for users synced with Azure AD Connect"

### fn spec.initProvider.withBusinessPhonesMixin

```ts
withBusinessPhonesMixin(businessPhones)
```

"A list of telephone numbers for the user. Only one number can be set for this property. Read-only for users synced with Azure AD Connect.\nThe telephone numbers for the user. Only one number can be set for this property. Read-only for users synced with Azure AD Connect"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withCity

```ts
withCity(city)
```

"The city in which the user is located.\nThe city in which the user is located"

### fn spec.initProvider.withCompanyName

```ts
withCompanyName(companyName)
```

"The company name which the user is associated. This property can be useful for describing the company that an external user comes from.\nThe company name which the user is associated. This property can be useful for describing the company that an external user comes from"

### fn spec.initProvider.withConsentProvidedForMinor

```ts
withConsentProvidedForMinor(consentProvidedForMinor)
```

"Whether consent has been obtained for minors. Supported values are Granted, Denied and NotRequired. Omit this property or specify a blank string to unset.\nWhether consent has been obtained for minors"

### fn spec.initProvider.withCostCenter

```ts
withCostCenter(costCenter)
```

"The cost center associated with the user.\nThe cost center associated with the user."

### fn spec.initProvider.withCountry

```ts
withCountry(country)
```

"The country/region in which the user is located. Examples include: NO, JP, and GB.\nThe country/region in which the user is located, e.g. `US` or `UK`"

### fn spec.initProvider.withDepartment

```ts
withDepartment(department)
```

"The name for the department in which the user works.\nThe name for the department in which the user works"

### fn spec.initProvider.withDisablePasswordExpiration

```ts
withDisablePasswordExpiration(disablePasswordExpiration)
```

"Whether the user's password is exempt from expiring. Defaults to false.\nWhether the users password is exempt from expiring"

### fn spec.initProvider.withDisableStrongPassword

```ts
withDisableStrongPassword(disableStrongPassword)
```

"Whether the user is allowed weaker passwords than the default policy to be specified. Defaults to false.\nWhether the user is allowed weaker passwords than the default policy to be specified."

### fn spec.initProvider.withDisplayName

```ts
withDisplayName(displayName)
```

"The name to display in the address book for the user.\nThe name to display in the address book for the user"

### fn spec.initProvider.withDivision

```ts
withDivision(division)
```

"The name of the division in which the user works.\nThe name of the division in which the user works."

### fn spec.initProvider.withEmployeeHireDate

```ts
withEmployeeHireDate(employeeHireDate)
```

"The hire date of the user, formatted as an RFC3339 date string (e.g. 2018-01-01T01:02:03Z).\nThe hire date of the user, formatted as an RFC3339 date string (e.g. `2018-01-01T01:02:03Z`)."

### fn spec.initProvider.withEmployeeId

```ts
withEmployeeId(employeeId)
```

"The employee identifier assigned to the user by the organisation.\nThe employee identifier assigned to the user by the organisation"

### fn spec.initProvider.withEmployeeType

```ts
withEmployeeType(employeeType)
```

"Captures enterprise worker type. For example, Employee, Contractor, Consultant, or Vendor.\nCaptures enterprise worker type. For example, Employee, Contractor, Consultant, or Vendor."

### fn spec.initProvider.withFaxNumber

```ts
withFaxNumber(faxNumber)
```

"The fax number of the user.\nThe fax number of the user"

### fn spec.initProvider.withForcePasswordChange

```ts
withForcePasswordChange(forcePasswordChange)
```

"Whether the user is forced to change the password during the next sign-in. Only takes effect when also changing the password. Defaults to false.\nWhether the user is forced to change the password during the next sign-in. Only takes effect when also changing the password"

### fn spec.initProvider.withGivenName

```ts
withGivenName(givenName)
```

"The given name (first name) of the user.\nThe given name (first name) of the user"

### fn spec.initProvider.withJobTitle

```ts
withJobTitle(jobTitle)
```

"The user’s job title.\nThe user’s job title"

### fn spec.initProvider.withMail

```ts
withMail(mail)
```

"The SMTP address for the user. This property cannot be unset once specified.\nThe SMTP address for the user. Cannot be unset."

### fn spec.initProvider.withMailNickname

```ts
withMailNickname(mailNickname)
```

"The mail alias for the user. Defaults to the user name part of the user principal name (UPN).\nThe mail alias for the user. Defaults to the user name part of the user principal name (UPN)"

### fn spec.initProvider.withManagerId

```ts
withManagerId(managerId)
```

"The object ID of the user's manager.\nThe object ID of the user's manager"

### fn spec.initProvider.withMobilePhone

```ts
withMobilePhone(mobilePhone)
```

"The primary cellular telephone number for the user.\nThe primary cellular telephone number for the user"

### fn spec.initProvider.withOfficeLocation

```ts
withOfficeLocation(officeLocation)
```

"The office location in the user's place of business.\nThe office location in the user's place of business"

### fn spec.initProvider.withOnpremisesImmutableId

```ts
withOnpremisesImmutableId(onpremisesImmutableId)
```

"The value used to associate an on-premise Active Directory user account with their Azure AD user object. This must be specified if you are using a federated domain for the user's user_principal_name property when creating a new user account.\nThe value used to associate an on-premise Active Directory user account with their Azure AD user object. This must be specified if you are using a federated domain for the user's `user_principal_name` property when creating a new user account"

### fn spec.initProvider.withOtherMails

```ts
withOtherMails(otherMails)
```

"A list of additional email addresses for the user.\nAdditional email addresses for the user"

### fn spec.initProvider.withOtherMailsMixin

```ts
withOtherMailsMixin(otherMails)
```

"A list of additional email addresses for the user.\nAdditional email addresses for the user"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withPostalCode

```ts
withPostalCode(postalCode)
```

"The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.\nThe postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code"

### fn spec.initProvider.withPreferredLanguage

```ts
withPreferredLanguage(preferredLanguage)
```

"The user's preferred language, in ISO 639-1 notation.\nThe user's preferred language, in ISO 639-1 notation"

### fn spec.initProvider.withShowInAddressList

```ts
withShowInAddressList(showInAddressList)
```

"Whether or not the Outlook global address list should include this user. Defaults to true.\nWhether or not the Outlook global address list should include this user"

### fn spec.initProvider.withState

```ts
withState(state)
```

"The state or province in the user's address.\nThe state or province in the user's address"

### fn spec.initProvider.withStreetAddress

```ts
withStreetAddress(streetAddress)
```

"The street address of the user's place of business.\nThe street address of the user's place of business"

### fn spec.initProvider.withSurname

```ts
withSurname(surname)
```

"The user's surname (family name or last name).\nThe user's surname (family name or last name)"

### fn spec.initProvider.withUsageLocation

```ts
withUsageLocation(usageLocation)
```

"The usage location of the user. Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries. The usage location is a two letter country code (ISO standard 3166). Examples include: NO, JP, and GB. Cannot be reset to null once set.\nThe usage location of the user. Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries. The usage location is a two letter country code (ISO standard 3166). Examples include: `NO`, `JP`, and `GB`. Cannot be reset to null once set"

### fn spec.initProvider.withUserPrincipalName

```ts
withUserPrincipalName(userPrincipalName)
```

"The user principal name (UPN) of the user.\nThe user principal name (UPN) of the user"

## obj spec.initProvider.passwordSecretRef

"The password for the user. The password must satisfy minimum requirements as specified by the password policy. The maximum length is 256 characters. This property is required when creating a new user.\nThe password for the user. The password must satisfy minimum requirements as specified by the password policy. The maximum length is 256 characters. This property is required when creating a new user"

### fn spec.initProvider.passwordSecretRef.withKey

```ts
withKey(key)
```

"The key to select."

### fn spec.initProvider.passwordSecretRef.withName

```ts
withName(name)
```

"Name of the secret."

### fn spec.initProvider.passwordSecretRef.withNamespace

```ts
withNamespace(namespace)
```

"Namespace of the secret."

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