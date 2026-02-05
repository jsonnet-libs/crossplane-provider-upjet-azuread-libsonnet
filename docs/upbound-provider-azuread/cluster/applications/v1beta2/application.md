---
permalink: /upbound-provider-azuread/cluster/applications/v1beta2/application/
---

# applications.v1beta2.application

"Application is the Schema for the Applications API."

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
    * [`fn withDescription(description)`](#fn-specforproviderwithdescription)
    * [`fn withDeviceOnlyAuthEnabled(deviceOnlyAuthEnabled)`](#fn-specforproviderwithdeviceonlyauthenabled)
    * [`fn withDisplayName(displayName)`](#fn-specforproviderwithdisplayname)
    * [`fn withFallbackPublicClientEnabled(fallbackPublicClientEnabled)`](#fn-specforproviderwithfallbackpublicclientenabled)
    * [`fn withFeatureTags(featureTags)`](#fn-specforproviderwithfeaturetags)
    * [`fn withFeatureTagsMixin(featureTags)`](#fn-specforproviderwithfeaturetagsmixin)
    * [`fn withGroupMembershipClaims(groupMembershipClaims)`](#fn-specforproviderwithgroupmembershipclaims)
    * [`fn withGroupMembershipClaimsMixin(groupMembershipClaims)`](#fn-specforproviderwithgroupmembershipclaimsmixin)
    * [`fn withIdentifierUris(identifierUris)`](#fn-specforproviderwithidentifieruris)
    * [`fn withIdentifierUrisMixin(identifierUris)`](#fn-specforproviderwithidentifierurismixin)
    * [`fn withLogoImage(logoImage)`](#fn-specforproviderwithlogoimage)
    * [`fn withMarketingUrl(marketingUrl)`](#fn-specforproviderwithmarketingurl)
    * [`fn withNotes(notes)`](#fn-specforproviderwithnotes)
    * [`fn withOauth2PostResponseRequired(oauth2PostResponseRequired)`](#fn-specforproviderwithoauth2postresponserequired)
    * [`fn withOwners(owners)`](#fn-specforproviderwithowners)
    * [`fn withOwnersMixin(owners)`](#fn-specforproviderwithownersmixin)
    * [`fn withPreventDuplicateNames(preventDuplicateNames)`](#fn-specforproviderwithpreventduplicatenames)
    * [`fn withPrivacyStatementUrl(privacyStatementUrl)`](#fn-specforproviderwithprivacystatementurl)
    * [`fn withRequiredResourceAccess(requiredResourceAccess)`](#fn-specforproviderwithrequiredresourceaccess)
    * [`fn withRequiredResourceAccessMixin(requiredResourceAccess)`](#fn-specforproviderwithrequiredresourceaccessmixin)
    * [`fn withServiceManagementReference(serviceManagementReference)`](#fn-specforproviderwithservicemanagementreference)
    * [`fn withSignInAudience(signInAudience)`](#fn-specforproviderwithsigninaudience)
    * [`fn withSupportUrl(supportUrl)`](#fn-specforproviderwithsupporturl)
    * [`fn withTags(tags)`](#fn-specforproviderwithtags)
    * [`fn withTagsMixin(tags)`](#fn-specforproviderwithtagsmixin)
    * [`fn withTemplateId(templateId)`](#fn-specforproviderwithtemplateid)
    * [`fn withTermsOfServiceUrl(termsOfServiceUrl)`](#fn-specforproviderwithtermsofserviceurl)
    * [`obj spec.forProvider.api`](#obj-specforproviderapi)
      * [`fn withKnownClientApplications(knownClientApplications)`](#fn-specforproviderapiwithknownclientapplications)
      * [`fn withKnownClientApplicationsMixin(knownClientApplications)`](#fn-specforproviderapiwithknownclientapplicationsmixin)
      * [`fn withKnownClientApplicationsRefs(knownClientApplicationsRefs)`](#fn-specforproviderapiwithknownclientapplicationsrefs)
      * [`fn withKnownClientApplicationsRefsMixin(knownClientApplicationsRefs)`](#fn-specforproviderapiwithknownclientapplicationsrefsmixin)
      * [`fn withMappedClaimsEnabled(mappedClaimsEnabled)`](#fn-specforproviderapiwithmappedclaimsenabled)
      * [`fn withOauth2PermissionScope(oauth2PermissionScope)`](#fn-specforproviderapiwithoauth2permissionscope)
      * [`fn withOauth2PermissionScopeMixin(oauth2PermissionScope)`](#fn-specforproviderapiwithoauth2permissionscopemixin)
      * [`fn withRequestedAccessTokenVersion(requestedAccessTokenVersion)`](#fn-specforproviderapiwithrequestedaccesstokenversion)
      * [`obj spec.forProvider.api.knownClientApplicationsRefs`](#obj-specforproviderapiknownclientapplicationsrefs)
        * [`fn withName(name)`](#fn-specforproviderapiknownclientapplicationsrefswithname)
        * [`obj spec.forProvider.api.knownClientApplicationsRefs.policy`](#obj-specforproviderapiknownclientapplicationsrefspolicy)
          * [`fn withResolution(resolution)`](#fn-specforproviderapiknownclientapplicationsrefspolicywithresolution)
          * [`fn withResolve(resolve)`](#fn-specforproviderapiknownclientapplicationsrefspolicywithresolve)
      * [`obj spec.forProvider.api.knownClientApplicationsSelector`](#obj-specforproviderapiknownclientapplicationsselector)
        * [`fn withMatchControllerRef(matchControllerRef)`](#fn-specforproviderapiknownclientapplicationsselectorwithmatchcontrollerref)
        * [`fn withMatchLabels(matchLabels)`](#fn-specforproviderapiknownclientapplicationsselectorwithmatchlabels)
        * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specforproviderapiknownclientapplicationsselectorwithmatchlabelsmixin)
        * [`obj spec.forProvider.api.knownClientApplicationsSelector.policy`](#obj-specforproviderapiknownclientapplicationsselectorpolicy)
          * [`fn withResolution(resolution)`](#fn-specforproviderapiknownclientapplicationsselectorpolicywithresolution)
          * [`fn withResolve(resolve)`](#fn-specforproviderapiknownclientapplicationsselectorpolicywithresolve)
      * [`obj spec.forProvider.api.oauth2PermissionScope`](#obj-specforproviderapioauth2permissionscope)
        * [`fn withAdminConsentDescription(adminConsentDescription)`](#fn-specforproviderapioauth2permissionscopewithadminconsentdescription)
        * [`fn withAdminConsentDisplayName(adminConsentDisplayName)`](#fn-specforproviderapioauth2permissionscopewithadminconsentdisplayname)
        * [`fn withEnabled(enabled)`](#fn-specforproviderapioauth2permissionscopewithenabled)
        * [`fn withId(id)`](#fn-specforproviderapioauth2permissionscopewithid)
        * [`fn withType(type)`](#fn-specforproviderapioauth2permissionscopewithtype)
        * [`fn withUserConsentDescription(userConsentDescription)`](#fn-specforproviderapioauth2permissionscopewithuserconsentdescription)
        * [`fn withUserConsentDisplayName(userConsentDisplayName)`](#fn-specforproviderapioauth2permissionscopewithuserconsentdisplayname)
        * [`fn withValue(value)`](#fn-specforproviderapioauth2permissionscopewithvalue)
    * [`obj spec.forProvider.featureTags`](#obj-specforproviderfeaturetags)
      * [`fn withCustomSingleSignOn(customSingleSignOn)`](#fn-specforproviderfeaturetagswithcustomsinglesignon)
      * [`fn withEnterprise(enterprise)`](#fn-specforproviderfeaturetagswithenterprise)
      * [`fn withGallery(gallery)`](#fn-specforproviderfeaturetagswithgallery)
      * [`fn withHide(hide)`](#fn-specforproviderfeaturetagswithhide)
    * [`obj spec.forProvider.optionalClaims`](#obj-specforprovideroptionalclaims)
      * [`fn withAccessToken(accessToken)`](#fn-specforprovideroptionalclaimswithaccesstoken)
      * [`fn withAccessTokenMixin(accessToken)`](#fn-specforprovideroptionalclaimswithaccesstokenmixin)
      * [`fn withIdToken(idToken)`](#fn-specforprovideroptionalclaimswithidtoken)
      * [`fn withIdTokenMixin(idToken)`](#fn-specforprovideroptionalclaimswithidtokenmixin)
      * [`fn withSaml2Token(saml2Token)`](#fn-specforprovideroptionalclaimswithsaml2token)
      * [`fn withSaml2TokenMixin(saml2Token)`](#fn-specforprovideroptionalclaimswithsaml2tokenmixin)
      * [`obj spec.forProvider.optionalClaims.accessToken`](#obj-specforprovideroptionalclaimsaccesstoken)
        * [`fn withAdditionalProperties(additionalProperties)`](#fn-specforprovideroptionalclaimsaccesstokenwithadditionalproperties)
        * [`fn withAdditionalPropertiesMixin(additionalProperties)`](#fn-specforprovideroptionalclaimsaccesstokenwithadditionalpropertiesmixin)
        * [`fn withEssential(essential)`](#fn-specforprovideroptionalclaimsaccesstokenwithessential)
        * [`fn withName(name)`](#fn-specforprovideroptionalclaimsaccesstokenwithname)
        * [`fn withSource(source)`](#fn-specforprovideroptionalclaimsaccesstokenwithsource)
      * [`obj spec.forProvider.optionalClaims.idToken`](#obj-specforprovideroptionalclaimsidtoken)
        * [`fn withAdditionalProperties(additionalProperties)`](#fn-specforprovideroptionalclaimsidtokenwithadditionalproperties)
        * [`fn withAdditionalPropertiesMixin(additionalProperties)`](#fn-specforprovideroptionalclaimsidtokenwithadditionalpropertiesmixin)
        * [`fn withEssential(essential)`](#fn-specforprovideroptionalclaimsidtokenwithessential)
        * [`fn withName(name)`](#fn-specforprovideroptionalclaimsidtokenwithname)
        * [`fn withSource(source)`](#fn-specforprovideroptionalclaimsidtokenwithsource)
      * [`obj spec.forProvider.optionalClaims.saml2Token`](#obj-specforprovideroptionalclaimssaml2token)
        * [`fn withAdditionalProperties(additionalProperties)`](#fn-specforprovideroptionalclaimssaml2tokenwithadditionalproperties)
        * [`fn withAdditionalPropertiesMixin(additionalProperties)`](#fn-specforprovideroptionalclaimssaml2tokenwithadditionalpropertiesmixin)
        * [`fn withEssential(essential)`](#fn-specforprovideroptionalclaimssaml2tokenwithessential)
        * [`fn withName(name)`](#fn-specforprovideroptionalclaimssaml2tokenwithname)
        * [`fn withSource(source)`](#fn-specforprovideroptionalclaimssaml2tokenwithsource)
    * [`obj spec.forProvider.password`](#obj-specforproviderpassword)
      * [`fn withDisplayName(displayName)`](#fn-specforproviderpasswordwithdisplayname)
      * [`fn withEndDate(endDate)`](#fn-specforproviderpasswordwithenddate)
      * [`fn withStartDate(startDate)`](#fn-specforproviderpasswordwithstartdate)
    * [`obj spec.forProvider.publicClient`](#obj-specforproviderpublicclient)
      * [`fn withRedirectUris(redirectUris)`](#fn-specforproviderpublicclientwithredirecturis)
      * [`fn withRedirectUrisMixin(redirectUris)`](#fn-specforproviderpublicclientwithredirecturismixin)
    * [`obj spec.forProvider.requiredResourceAccess`](#obj-specforproviderrequiredresourceaccess)
      * [`fn withResourceAccess(resourceAccess)`](#fn-specforproviderrequiredresourceaccesswithresourceaccess)
      * [`fn withResourceAccessMixin(resourceAccess)`](#fn-specforproviderrequiredresourceaccesswithresourceaccessmixin)
      * [`fn withResourceAppId(resourceAppId)`](#fn-specforproviderrequiredresourceaccesswithresourceappid)
      * [`obj spec.forProvider.requiredResourceAccess.resourceAccess`](#obj-specforproviderrequiredresourceaccessresourceaccess)
        * [`fn withId(id)`](#fn-specforproviderrequiredresourceaccessresourceaccesswithid)
        * [`fn withType(type)`](#fn-specforproviderrequiredresourceaccessresourceaccesswithtype)
    * [`obj spec.forProvider.singlePageApplication`](#obj-specforprovidersinglepageapplication)
      * [`fn withRedirectUris(redirectUris)`](#fn-specforprovidersinglepageapplicationwithredirecturis)
      * [`fn withRedirectUrisMixin(redirectUris)`](#fn-specforprovidersinglepageapplicationwithredirecturismixin)
    * [`obj spec.forProvider.web`](#obj-specforproviderweb)
      * [`fn withHomepageUrl(homepageUrl)`](#fn-specforproviderwebwithhomepageurl)
      * [`fn withLogoutUrl(logoutUrl)`](#fn-specforproviderwebwithlogouturl)
      * [`fn withRedirectUris(redirectUris)`](#fn-specforproviderwebwithredirecturis)
      * [`fn withRedirectUrisMixin(redirectUris)`](#fn-specforproviderwebwithredirecturismixin)
      * [`obj spec.forProvider.web.implicitGrant`](#obj-specforproviderwebimplicitgrant)
        * [`fn withAccessTokenIssuanceEnabled(accessTokenIssuanceEnabled)`](#fn-specforproviderwebimplicitgrantwithaccesstokenissuanceenabled)
        * [`fn withIdTokenIssuanceEnabled(idTokenIssuanceEnabled)`](#fn-specforproviderwebimplicitgrantwithidtokenissuanceenabled)
  * [`obj spec.initProvider`](#obj-specinitprovider)
    * [`fn withDescription(description)`](#fn-specinitproviderwithdescription)
    * [`fn withDeviceOnlyAuthEnabled(deviceOnlyAuthEnabled)`](#fn-specinitproviderwithdeviceonlyauthenabled)
    * [`fn withDisplayName(displayName)`](#fn-specinitproviderwithdisplayname)
    * [`fn withFallbackPublicClientEnabled(fallbackPublicClientEnabled)`](#fn-specinitproviderwithfallbackpublicclientenabled)
    * [`fn withFeatureTags(featureTags)`](#fn-specinitproviderwithfeaturetags)
    * [`fn withFeatureTagsMixin(featureTags)`](#fn-specinitproviderwithfeaturetagsmixin)
    * [`fn withGroupMembershipClaims(groupMembershipClaims)`](#fn-specinitproviderwithgroupmembershipclaims)
    * [`fn withGroupMembershipClaimsMixin(groupMembershipClaims)`](#fn-specinitproviderwithgroupmembershipclaimsmixin)
    * [`fn withIdentifierUris(identifierUris)`](#fn-specinitproviderwithidentifieruris)
    * [`fn withIdentifierUrisMixin(identifierUris)`](#fn-specinitproviderwithidentifierurismixin)
    * [`fn withLogoImage(logoImage)`](#fn-specinitproviderwithlogoimage)
    * [`fn withMarketingUrl(marketingUrl)`](#fn-specinitproviderwithmarketingurl)
    * [`fn withNotes(notes)`](#fn-specinitproviderwithnotes)
    * [`fn withOauth2PostResponseRequired(oauth2PostResponseRequired)`](#fn-specinitproviderwithoauth2postresponserequired)
    * [`fn withOwners(owners)`](#fn-specinitproviderwithowners)
    * [`fn withOwnersMixin(owners)`](#fn-specinitproviderwithownersmixin)
    * [`fn withPreventDuplicateNames(preventDuplicateNames)`](#fn-specinitproviderwithpreventduplicatenames)
    * [`fn withPrivacyStatementUrl(privacyStatementUrl)`](#fn-specinitproviderwithprivacystatementurl)
    * [`fn withRequiredResourceAccess(requiredResourceAccess)`](#fn-specinitproviderwithrequiredresourceaccess)
    * [`fn withRequiredResourceAccessMixin(requiredResourceAccess)`](#fn-specinitproviderwithrequiredresourceaccessmixin)
    * [`fn withServiceManagementReference(serviceManagementReference)`](#fn-specinitproviderwithservicemanagementreference)
    * [`fn withSignInAudience(signInAudience)`](#fn-specinitproviderwithsigninaudience)
    * [`fn withSupportUrl(supportUrl)`](#fn-specinitproviderwithsupporturl)
    * [`fn withTags(tags)`](#fn-specinitproviderwithtags)
    * [`fn withTagsMixin(tags)`](#fn-specinitproviderwithtagsmixin)
    * [`fn withTemplateId(templateId)`](#fn-specinitproviderwithtemplateid)
    * [`fn withTermsOfServiceUrl(termsOfServiceUrl)`](#fn-specinitproviderwithtermsofserviceurl)
    * [`obj spec.initProvider.api`](#obj-specinitproviderapi)
      * [`fn withKnownClientApplications(knownClientApplications)`](#fn-specinitproviderapiwithknownclientapplications)
      * [`fn withKnownClientApplicationsMixin(knownClientApplications)`](#fn-specinitproviderapiwithknownclientapplicationsmixin)
      * [`fn withKnownClientApplicationsRefs(knownClientApplicationsRefs)`](#fn-specinitproviderapiwithknownclientapplicationsrefs)
      * [`fn withKnownClientApplicationsRefsMixin(knownClientApplicationsRefs)`](#fn-specinitproviderapiwithknownclientapplicationsrefsmixin)
      * [`fn withMappedClaimsEnabled(mappedClaimsEnabled)`](#fn-specinitproviderapiwithmappedclaimsenabled)
      * [`fn withOauth2PermissionScope(oauth2PermissionScope)`](#fn-specinitproviderapiwithoauth2permissionscope)
      * [`fn withOauth2PermissionScopeMixin(oauth2PermissionScope)`](#fn-specinitproviderapiwithoauth2permissionscopemixin)
      * [`fn withRequestedAccessTokenVersion(requestedAccessTokenVersion)`](#fn-specinitproviderapiwithrequestedaccesstokenversion)
      * [`obj spec.initProvider.api.knownClientApplicationsRefs`](#obj-specinitproviderapiknownclientapplicationsrefs)
        * [`fn withName(name)`](#fn-specinitproviderapiknownclientapplicationsrefswithname)
        * [`obj spec.initProvider.api.knownClientApplicationsRefs.policy`](#obj-specinitproviderapiknownclientapplicationsrefspolicy)
          * [`fn withResolution(resolution)`](#fn-specinitproviderapiknownclientapplicationsrefspolicywithresolution)
          * [`fn withResolve(resolve)`](#fn-specinitproviderapiknownclientapplicationsrefspolicywithresolve)
      * [`obj spec.initProvider.api.knownClientApplicationsSelector`](#obj-specinitproviderapiknownclientapplicationsselector)
        * [`fn withMatchControllerRef(matchControllerRef)`](#fn-specinitproviderapiknownclientapplicationsselectorwithmatchcontrollerref)
        * [`fn withMatchLabels(matchLabels)`](#fn-specinitproviderapiknownclientapplicationsselectorwithmatchlabels)
        * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specinitproviderapiknownclientapplicationsselectorwithmatchlabelsmixin)
        * [`obj spec.initProvider.api.knownClientApplicationsSelector.policy`](#obj-specinitproviderapiknownclientapplicationsselectorpolicy)
          * [`fn withResolution(resolution)`](#fn-specinitproviderapiknownclientapplicationsselectorpolicywithresolution)
          * [`fn withResolve(resolve)`](#fn-specinitproviderapiknownclientapplicationsselectorpolicywithresolve)
      * [`obj spec.initProvider.api.oauth2PermissionScope`](#obj-specinitproviderapioauth2permissionscope)
        * [`fn withAdminConsentDescription(adminConsentDescription)`](#fn-specinitproviderapioauth2permissionscopewithadminconsentdescription)
        * [`fn withAdminConsentDisplayName(adminConsentDisplayName)`](#fn-specinitproviderapioauth2permissionscopewithadminconsentdisplayname)
        * [`fn withEnabled(enabled)`](#fn-specinitproviderapioauth2permissionscopewithenabled)
        * [`fn withId(id)`](#fn-specinitproviderapioauth2permissionscopewithid)
        * [`fn withType(type)`](#fn-specinitproviderapioauth2permissionscopewithtype)
        * [`fn withUserConsentDescription(userConsentDescription)`](#fn-specinitproviderapioauth2permissionscopewithuserconsentdescription)
        * [`fn withUserConsentDisplayName(userConsentDisplayName)`](#fn-specinitproviderapioauth2permissionscopewithuserconsentdisplayname)
        * [`fn withValue(value)`](#fn-specinitproviderapioauth2permissionscopewithvalue)
    * [`obj spec.initProvider.featureTags`](#obj-specinitproviderfeaturetags)
      * [`fn withCustomSingleSignOn(customSingleSignOn)`](#fn-specinitproviderfeaturetagswithcustomsinglesignon)
      * [`fn withEnterprise(enterprise)`](#fn-specinitproviderfeaturetagswithenterprise)
      * [`fn withGallery(gallery)`](#fn-specinitproviderfeaturetagswithgallery)
      * [`fn withHide(hide)`](#fn-specinitproviderfeaturetagswithhide)
    * [`obj spec.initProvider.optionalClaims`](#obj-specinitprovideroptionalclaims)
      * [`fn withAccessToken(accessToken)`](#fn-specinitprovideroptionalclaimswithaccesstoken)
      * [`fn withAccessTokenMixin(accessToken)`](#fn-specinitprovideroptionalclaimswithaccesstokenmixin)
      * [`fn withIdToken(idToken)`](#fn-specinitprovideroptionalclaimswithidtoken)
      * [`fn withIdTokenMixin(idToken)`](#fn-specinitprovideroptionalclaimswithidtokenmixin)
      * [`fn withSaml2Token(saml2Token)`](#fn-specinitprovideroptionalclaimswithsaml2token)
      * [`fn withSaml2TokenMixin(saml2Token)`](#fn-specinitprovideroptionalclaimswithsaml2tokenmixin)
      * [`obj spec.initProvider.optionalClaims.accessToken`](#obj-specinitprovideroptionalclaimsaccesstoken)
        * [`fn withAdditionalProperties(additionalProperties)`](#fn-specinitprovideroptionalclaimsaccesstokenwithadditionalproperties)
        * [`fn withAdditionalPropertiesMixin(additionalProperties)`](#fn-specinitprovideroptionalclaimsaccesstokenwithadditionalpropertiesmixin)
        * [`fn withEssential(essential)`](#fn-specinitprovideroptionalclaimsaccesstokenwithessential)
        * [`fn withName(name)`](#fn-specinitprovideroptionalclaimsaccesstokenwithname)
        * [`fn withSource(source)`](#fn-specinitprovideroptionalclaimsaccesstokenwithsource)
      * [`obj spec.initProvider.optionalClaims.idToken`](#obj-specinitprovideroptionalclaimsidtoken)
        * [`fn withAdditionalProperties(additionalProperties)`](#fn-specinitprovideroptionalclaimsidtokenwithadditionalproperties)
        * [`fn withAdditionalPropertiesMixin(additionalProperties)`](#fn-specinitprovideroptionalclaimsidtokenwithadditionalpropertiesmixin)
        * [`fn withEssential(essential)`](#fn-specinitprovideroptionalclaimsidtokenwithessential)
        * [`fn withName(name)`](#fn-specinitprovideroptionalclaimsidtokenwithname)
        * [`fn withSource(source)`](#fn-specinitprovideroptionalclaimsidtokenwithsource)
      * [`obj spec.initProvider.optionalClaims.saml2Token`](#obj-specinitprovideroptionalclaimssaml2token)
        * [`fn withAdditionalProperties(additionalProperties)`](#fn-specinitprovideroptionalclaimssaml2tokenwithadditionalproperties)
        * [`fn withAdditionalPropertiesMixin(additionalProperties)`](#fn-specinitprovideroptionalclaimssaml2tokenwithadditionalpropertiesmixin)
        * [`fn withEssential(essential)`](#fn-specinitprovideroptionalclaimssaml2tokenwithessential)
        * [`fn withName(name)`](#fn-specinitprovideroptionalclaimssaml2tokenwithname)
        * [`fn withSource(source)`](#fn-specinitprovideroptionalclaimssaml2tokenwithsource)
    * [`obj spec.initProvider.password`](#obj-specinitproviderpassword)
      * [`fn withDisplayName(displayName)`](#fn-specinitproviderpasswordwithdisplayname)
      * [`fn withEndDate(endDate)`](#fn-specinitproviderpasswordwithenddate)
      * [`fn withStartDate(startDate)`](#fn-specinitproviderpasswordwithstartdate)
    * [`obj spec.initProvider.publicClient`](#obj-specinitproviderpublicclient)
      * [`fn withRedirectUris(redirectUris)`](#fn-specinitproviderpublicclientwithredirecturis)
      * [`fn withRedirectUrisMixin(redirectUris)`](#fn-specinitproviderpublicclientwithredirecturismixin)
    * [`obj spec.initProvider.requiredResourceAccess`](#obj-specinitproviderrequiredresourceaccess)
      * [`fn withResourceAccess(resourceAccess)`](#fn-specinitproviderrequiredresourceaccesswithresourceaccess)
      * [`fn withResourceAccessMixin(resourceAccess)`](#fn-specinitproviderrequiredresourceaccesswithresourceaccessmixin)
      * [`fn withResourceAppId(resourceAppId)`](#fn-specinitproviderrequiredresourceaccesswithresourceappid)
      * [`obj spec.initProvider.requiredResourceAccess.resourceAccess`](#obj-specinitproviderrequiredresourceaccessresourceaccess)
        * [`fn withId(id)`](#fn-specinitproviderrequiredresourceaccessresourceaccesswithid)
        * [`fn withType(type)`](#fn-specinitproviderrequiredresourceaccessresourceaccesswithtype)
    * [`obj spec.initProvider.singlePageApplication`](#obj-specinitprovidersinglepageapplication)
      * [`fn withRedirectUris(redirectUris)`](#fn-specinitprovidersinglepageapplicationwithredirecturis)
      * [`fn withRedirectUrisMixin(redirectUris)`](#fn-specinitprovidersinglepageapplicationwithredirecturismixin)
    * [`obj spec.initProvider.web`](#obj-specinitproviderweb)
      * [`fn withHomepageUrl(homepageUrl)`](#fn-specinitproviderwebwithhomepageurl)
      * [`fn withLogoutUrl(logoutUrl)`](#fn-specinitproviderwebwithlogouturl)
      * [`fn withRedirectUris(redirectUris)`](#fn-specinitproviderwebwithredirecturis)
      * [`fn withRedirectUrisMixin(redirectUris)`](#fn-specinitproviderwebwithredirecturismixin)
      * [`obj spec.initProvider.web.implicitGrant`](#obj-specinitproviderwebimplicitgrant)
        * [`fn withAccessTokenIssuanceEnabled(accessTokenIssuanceEnabled)`](#fn-specinitproviderwebimplicitgrantwithaccesstokenissuanceenabled)
        * [`fn withIdTokenIssuanceEnabled(idTokenIssuanceEnabled)`](#fn-specinitproviderwebimplicitgrantwithidtokenissuanceenabled)
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

new returns an instance of Application

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

"ApplicationSpec defines the desired state of Application"

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



### fn spec.forProvider.withDescription

```ts
withDescription(description)
```

"A description of the application, as shown to end users.\nDescription of the application as shown to end users"

### fn spec.forProvider.withDeviceOnlyAuthEnabled

```ts
withDeviceOnlyAuthEnabled(deviceOnlyAuthEnabled)
```

"Specifies whether this application supports device authentication without a user. Defaults to false.\nSpecifies whether this application supports device authentication without a user."

### fn spec.forProvider.withDisplayName

```ts
withDisplayName(displayName)
```

"The display name for the application.\nThe display name for the application"

### fn spec.forProvider.withFallbackPublicClientEnabled

```ts
withFallbackPublicClientEnabled(fallbackPublicClientEnabled)
```

"Specifies whether the application is a public client. Appropriate for apps using token grant flows that don't use a redirect URI. Defaults to false.\nSpecifies whether the application is a public client. Appropriate for apps using token grant flows that don't use a redirect URI"

### fn spec.forProvider.withFeatureTags

```ts
withFeatureTags(featureTags)
```

"A feature_tags block as described below. Cannot be used together with the tags property.\nBlock of features to configure for this application using tags"

### fn spec.forProvider.withFeatureTagsMixin

```ts
withFeatureTagsMixin(featureTags)
```

"A feature_tags block as described below. Cannot be used together with the tags property.\nBlock of features to configure for this application using tags"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withGroupMembershipClaims

```ts
withGroupMembershipClaims(groupMembershipClaims)
```

"A set of strings containing membership claims issued in a user or OAuth 2.0 access token that the app expects. Possible values are None, SecurityGroup, DirectoryRole, ApplicationGroup or All.\nConfigures the `groups` claim issued in a user or OAuth 2.0 access token that the app expects"

### fn spec.forProvider.withGroupMembershipClaimsMixin

```ts
withGroupMembershipClaimsMixin(groupMembershipClaims)
```

"A set of strings containing membership claims issued in a user or OAuth 2.0 access token that the app expects. Possible values are None, SecurityGroup, DirectoryRole, ApplicationGroup or All.\nConfigures the `groups` claim issued in a user or OAuth 2.0 access token that the app expects"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withIdentifierUris

```ts
withIdentifierUris(identifierUris)
```

"A set of user-defined URI(s) that uniquely identify an application within its Azure AD tenant, or within a verified custom domain if the application is multi-tenant.\nThe user-defined URI(s) that uniquely identify an application within its Azure AD tenant, or within a verified custom domain if the application is multi-tenant"

### fn spec.forProvider.withIdentifierUrisMixin

```ts
withIdentifierUrisMixin(identifierUris)
```

"A set of user-defined URI(s) that uniquely identify an application within its Azure AD tenant, or within a verified custom domain if the application is multi-tenant.\nThe user-defined URI(s) that uniquely identify an application within its Azure AD tenant, or within a verified custom domain if the application is multi-tenant"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withLogoImage

```ts
withLogoImage(logoImage)
```

"A logo image to upload for the application, as a raw base64-encoded string. The image should be in gif, jpeg or png format. Note that once an image has been uploaded, it is not possible to remove it without replacing it with another image.\nBase64 encoded logo image in gif, png or jpeg format"

### fn spec.forProvider.withMarketingUrl

```ts
withMarketingUrl(marketingUrl)
```

"URL of the application's marketing page.\nURL of the application's marketing page"

### fn spec.forProvider.withNotes

```ts
withNotes(notes)
```

"User-specified notes relevant for the management of the application.\nUser-specified notes relevant for the management of the application"

### fn spec.forProvider.withOauth2PostResponseRequired

```ts
withOauth2PostResponseRequired(oauth2PostResponseRequired)
```

"Specifies whether, as part of OAuth 2.0 token requests, Azure AD allows POST requests, as opposed to GET requests. Defaults to false, which specifies that only GET requests are allowed.\nSpecifies whether, as part of OAuth 2.0 token requests, Azure AD allows POST requests, as opposed to GET requests."

### fn spec.forProvider.withOwners

```ts
withOwners(owners)
```

"A set of object IDs of principals that will be granted ownership of the application. Supported object types are users or service principals. By default, no owners are assigned.\nA list of object IDs of principals that will be granted ownership of the application"

### fn spec.forProvider.withOwnersMixin

```ts
withOwnersMixin(owners)
```

"A set of object IDs of principals that will be granted ownership of the application. Supported object types are users or service principals. By default, no owners are assigned.\nA list of object IDs of principals that will be granted ownership of the application"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withPreventDuplicateNames

```ts
withPreventDuplicateNames(preventDuplicateNames)
```

"If true, will return an error if an existing application is found with the same name. Defaults to false.\nIf `true`, will return an error if an existing application is found with the same name"

### fn spec.forProvider.withPrivacyStatementUrl

```ts
withPrivacyStatementUrl(privacyStatementUrl)
```

"URL of the application's privacy statement.\nURL of the application's privacy statement"

### fn spec.forProvider.withRequiredResourceAccess

```ts
withRequiredResourceAccess(requiredResourceAccess)
```

"A collection of required_resource_access blocks as documented below."

### fn spec.forProvider.withRequiredResourceAccessMixin

```ts
withRequiredResourceAccessMixin(requiredResourceAccess)
```

"A collection of required_resource_access blocks as documented below."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withServiceManagementReference

```ts
withServiceManagementReference(serviceManagementReference)
```

"References application context information from a Service or Asset Management database.\nReferences application or service contact information from a Service or Asset Management database"

### fn spec.forProvider.withSignInAudience

```ts
withSignInAudience(signInAudience)
```

"The Microsoft account types that are supported for the current application. Must be one of AzureADMyOrg, AzureADMultipleOrgs, AzureADandPersonalMicrosoftAccount or PersonalMicrosoftAccount. Defaults to AzureADMyOrg.\nThe Microsoft account types that are supported for the current application"

### fn spec.forProvider.withSupportUrl

```ts
withSupportUrl(supportUrl)
```

"URL of the application's support page.\nURL of the application's support page"

### fn spec.forProvider.withTags

```ts
withTags(tags)
```

"A set of tags to apply to the application for configuring specific behaviours of the application and linked service principals. Note that these are not provided for use by practitioners. Cannot be used together with the feature_tags block.\nA set of tags to apply to the application"

### fn spec.forProvider.withTagsMixin

```ts
withTagsMixin(tags)
```

"A set of tags to apply to the application for configuring specific behaviours of the application and linked service principals. Note that these are not provided for use by practitioners. Cannot be used together with the feature_tags block.\nA set of tags to apply to the application"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withTemplateId

```ts
withTemplateId(templateId)
```

"Unique ID for a templated application in the Azure AD App Gallery, from which to create the application. Changing this forces a new resource to be created.\nUnique ID of the application template from which this application is created"

### fn spec.forProvider.withTermsOfServiceUrl

```ts
withTermsOfServiceUrl(termsOfServiceUrl)
```

"URL of the application's terms of service statement.\nURL of the application's terms of service statement"

## obj spec.forProvider.api

"An api block as documented below, which configures API related settings for this application."

### fn spec.forProvider.api.withKnownClientApplications

```ts
withKnownClientApplications(knownClientApplications)
```

"A set of client IDs, used for bundling consent if you have a solution that contains two parts: a client app and a custom web API app.\nUsed for bundling consent if you have a solution that contains two parts: a client app and a custom web API app"

### fn spec.forProvider.api.withKnownClientApplicationsMixin

```ts
withKnownClientApplicationsMixin(knownClientApplications)
```

"A set of client IDs, used for bundling consent if you have a solution that contains two parts: a client app and a custom web API app.\nUsed for bundling consent if you have a solution that contains two parts: a client app and a custom web API app"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.api.withKnownClientApplicationsRefs

```ts
withKnownClientApplicationsRefs(knownClientApplicationsRefs)
```

"References to Application in applications to populate knownClientApplications."

### fn spec.forProvider.api.withKnownClientApplicationsRefsMixin

```ts
withKnownClientApplicationsRefsMixin(knownClientApplicationsRefs)
```

"References to Application in applications to populate knownClientApplications."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.api.withMappedClaimsEnabled

```ts
withMappedClaimsEnabled(mappedClaimsEnabled)
```

"Allows an application to use claims mapping without specifying a custom signing key. Defaults to false.\nAllows an application to use claims mapping without specifying a custom signing key"

### fn spec.forProvider.api.withOauth2PermissionScope

```ts
withOauth2PermissionScope(oauth2PermissionScope)
```

"One or more oauth2_permission_scope blocks as documented below, to describe delegated permissions exposed by the web API represented by this application.\nOne or more `oauth2_permission_scope` blocks to describe delegated permissions exposed by the web API represented by this application"

### fn spec.forProvider.api.withOauth2PermissionScopeMixin

```ts
withOauth2PermissionScopeMixin(oauth2PermissionScope)
```

"One or more oauth2_permission_scope blocks as documented below, to describe delegated permissions exposed by the web API represented by this application.\nOne or more `oauth2_permission_scope` blocks to describe delegated permissions exposed by the web API represented by this application"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.api.withRequestedAccessTokenVersion

```ts
withRequestedAccessTokenVersion(requestedAccessTokenVersion)
```

"The access token version expected by this resource. Must be one of 1 or 2, and must be 2 when sign_in_audience is either AzureADandPersonalMicrosoftAccount or PersonalMicrosoftAccount Defaults to 1.\nThe access token version expected by this resource"

## obj spec.forProvider.api.knownClientApplicationsRefs

"References to Application in applications to populate knownClientApplications."

### fn spec.forProvider.api.knownClientApplicationsRefs.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.forProvider.api.knownClientApplicationsRefs.policy

"Policies for referencing."

### fn spec.forProvider.api.knownClientApplicationsRefs.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.forProvider.api.knownClientApplicationsRefs.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.forProvider.api.knownClientApplicationsSelector

"Selector for a list of Application in applications to populate knownClientApplications."

### fn spec.forProvider.api.knownClientApplicationsSelector.withMatchControllerRef

```ts
withMatchControllerRef(matchControllerRef)
```

"MatchControllerRef ensures an object with the same controller reference\nas the selecting object is selected."

### fn spec.forProvider.api.knownClientApplicationsSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

### fn spec.forProvider.api.knownClientApplicationsSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.api.knownClientApplicationsSelector.policy

"Policies for selection."

### fn spec.forProvider.api.knownClientApplicationsSelector.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.forProvider.api.knownClientApplicationsSelector.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.forProvider.api.oauth2PermissionScope

"One or more oauth2_permission_scope blocks as documented below, to describe delegated permissions exposed by the web API represented by this application.\nOne or more `oauth2_permission_scope` blocks to describe delegated permissions exposed by the web API represented by this application"

### fn spec.forProvider.api.oauth2PermissionScope.withAdminConsentDescription

```ts
withAdminConsentDescription(adminConsentDescription)
```

"Delegated permission description that appears in all tenant-wide admin consent experiences, intended to be read by an administrator granting the permission on behalf of all users.\nDelegated permission description that appears in all tenant-wide admin consent experiences, intended to be read by an administrator granting the permission on behalf of all users"

### fn spec.forProvider.api.oauth2PermissionScope.withAdminConsentDisplayName

```ts
withAdminConsentDisplayName(adminConsentDisplayName)
```

"Display name for the delegated permission, intended to be read by an administrator granting the permission on behalf of all users.\nDisplay name for the delegated permission, intended to be read by an administrator granting the permission on behalf of all users"

### fn spec.forProvider.api.oauth2PermissionScope.withEnabled

```ts
withEnabled(enabled)
```

"Determines if the permission scope is enabled. Defaults to true.\nDetermines if the permission scope is enabled"

### fn spec.forProvider.api.oauth2PermissionScope.withId

```ts
withId(id)
```

"The unique identifier of the delegated permission. Must be a valid UUID.\nThe unique identifier of the delegated permission"

### fn spec.forProvider.api.oauth2PermissionScope.withType

```ts
withType(type)
```

"Whether this delegated permission should be considered safe for non-admin users to consent to on behalf of themselves, or whether an administrator should be required for consent to the permissions. Defaults to User. Possible values are User or Admin.\nWhether this delegated permission should be considered safe for non-admin users to consent to on behalf of themselves, or whether an administrator should be required for consent to the permissions"

### fn spec.forProvider.api.oauth2PermissionScope.withUserConsentDescription

```ts
withUserConsentDescription(userConsentDescription)
```

"Delegated permission description that appears in the end user consent experience, intended to be read by a user consenting on their own behalf.\nDelegated permission description that appears in the end user consent experience, intended to be read by a user consenting on their own behalf"

### fn spec.forProvider.api.oauth2PermissionScope.withUserConsentDisplayName

```ts
withUserConsentDisplayName(userConsentDisplayName)
```

"Display name for the delegated permission that appears in the end user consent experience.\nDisplay name for the delegated permission that appears in the end user consent experience"

### fn spec.forProvider.api.oauth2PermissionScope.withValue

```ts
withValue(value)
```

"The value that is used for the scp claim in OAuth 2.0 access tokens.\nThe value that is used for the `scp` claim in OAuth 2.0 access tokens"

## obj spec.forProvider.featureTags

"A feature_tags block as described below. Cannot be used together with the tags property.\nBlock of features to configure for this application using tags"

### fn spec.forProvider.featureTags.withCustomSingleSignOn

```ts
withCustomSingleSignOn(customSingleSignOn)
```

"Whether this application represents a custom SAML application for linked service principals. Enabling this will assign the WindowsAzureActiveDirectoryCustomSingleSignOnApplication tag. Defaults to false.\nWhether this application represents a custom SAML application for linked service principals"

### fn spec.forProvider.featureTags.withEnterprise

```ts
withEnterprise(enterprise)
```

"Whether this application represents an Enterprise Application for linked service principals. Enabling this will assign the WindowsAzureActiveDirectoryIntegratedApp tag. Defaults to false.\nWhether this application represents an Enterprise Application for linked service principals"

### fn spec.forProvider.featureTags.withGallery

```ts
withGallery(gallery)
```

"Whether this application represents a gallery application for linked service principals. Enabling this will assign the WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1 tag. Defaults to false.\nWhether this application represents a gallery application for linked service principals"

### fn spec.forProvider.featureTags.withHide

```ts
withHide(hide)
```

"Whether this app is invisible to users in My Apps and Office 365 Launcher. Enabling this will assign the HideApp tag. Defaults to false.\nWhether this application is invisible to users in My Apps and Office 365 Launcher"

## obj spec.forProvider.optionalClaims

"An optional_claims block as documented below."

### fn spec.forProvider.optionalClaims.withAccessToken

```ts
withAccessToken(accessToken)
```

"One or more access_token blocks as documented below."

### fn spec.forProvider.optionalClaims.withAccessTokenMixin

```ts
withAccessTokenMixin(accessToken)
```

"One or more access_token blocks as documented below."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.optionalClaims.withIdToken

```ts
withIdToken(idToken)
```

"One or more id_token blocks as documented below."

### fn spec.forProvider.optionalClaims.withIdTokenMixin

```ts
withIdTokenMixin(idToken)
```

"One or more id_token blocks as documented below."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.optionalClaims.withSaml2Token

```ts
withSaml2Token(saml2Token)
```

"One or more saml2_token blocks as documented below."

### fn spec.forProvider.optionalClaims.withSaml2TokenMixin

```ts
withSaml2TokenMixin(saml2Token)
```

"One or more saml2_token blocks as documented below."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.optionalClaims.accessToken

"One or more access_token blocks as documented below."

### fn spec.forProvider.optionalClaims.accessToken.withAdditionalProperties

```ts
withAdditionalProperties(additionalProperties)
```

"List of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim. Possible values are: cloud_displayname, dns_domain_and_sam_account_name, emit_as_roles, include_externally_authenticated_upn_without_hash, include_externally_authenticated_upn, max_size_limit, netbios_domain_and_sam_account_name, on_premise_security_identifier, sam_account_name, and use_guid.\nList of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim"

### fn spec.forProvider.optionalClaims.accessToken.withAdditionalPropertiesMixin

```ts
withAdditionalPropertiesMixin(additionalProperties)
```

"List of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim. Possible values are: cloud_displayname, dns_domain_and_sam_account_name, emit_as_roles, include_externally_authenticated_upn_without_hash, include_externally_authenticated_upn, max_size_limit, netbios_domain_and_sam_account_name, on_premise_security_identifier, sam_account_name, and use_guid.\nList of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.optionalClaims.accessToken.withEssential

```ts
withEssential(essential)
```

"Whether the claim specified by the client is necessary to ensure a smooth authorization experience.\nWhether the claim specified by the client is necessary to ensure a smooth authorization experience"

### fn spec.forProvider.optionalClaims.accessToken.withName

```ts
withName(name)
```

"The name of the optional claim.\nThe name of the optional claim"

### fn spec.forProvider.optionalClaims.accessToken.withSource

```ts
withSource(source)
```

"The source of the claim. If source is absent, the claim is a predefined optional claim. If source is user, the value of name is the extension property from the user object.\nThe source of the claim. If `source` is absent, the claim is a predefined optional claim. If `source` is `user`, the value of `name` is the extension property from the user object"

## obj spec.forProvider.optionalClaims.idToken

"One or more id_token blocks as documented below."

### fn spec.forProvider.optionalClaims.idToken.withAdditionalProperties

```ts
withAdditionalProperties(additionalProperties)
```

"List of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim. Possible values are: cloud_displayname, dns_domain_and_sam_account_name, emit_as_roles, include_externally_authenticated_upn_without_hash, include_externally_authenticated_upn, max_size_limit, netbios_domain_and_sam_account_name, on_premise_security_identifier, sam_account_name, and use_guid.\nList of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim"

### fn spec.forProvider.optionalClaims.idToken.withAdditionalPropertiesMixin

```ts
withAdditionalPropertiesMixin(additionalProperties)
```

"List of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim. Possible values are: cloud_displayname, dns_domain_and_sam_account_name, emit_as_roles, include_externally_authenticated_upn_without_hash, include_externally_authenticated_upn, max_size_limit, netbios_domain_and_sam_account_name, on_premise_security_identifier, sam_account_name, and use_guid.\nList of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.optionalClaims.idToken.withEssential

```ts
withEssential(essential)
```

"Whether the claim specified by the client is necessary to ensure a smooth authorization experience.\nWhether the claim specified by the client is necessary to ensure a smooth authorization experience"

### fn spec.forProvider.optionalClaims.idToken.withName

```ts
withName(name)
```

"The name of the optional claim.\nThe name of the optional claim"

### fn spec.forProvider.optionalClaims.idToken.withSource

```ts
withSource(source)
```

"The source of the claim. If source is absent, the claim is a predefined optional claim. If source is user, the value of name is the extension property from the user object.\nThe source of the claim. If `source` is absent, the claim is a predefined optional claim. If `source` is `user`, the value of `name` is the extension property from the user object"

## obj spec.forProvider.optionalClaims.saml2Token

"One or more saml2_token blocks as documented below."

### fn spec.forProvider.optionalClaims.saml2Token.withAdditionalProperties

```ts
withAdditionalProperties(additionalProperties)
```

"List of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim. Possible values are: cloud_displayname, dns_domain_and_sam_account_name, emit_as_roles, include_externally_authenticated_upn_without_hash, include_externally_authenticated_upn, max_size_limit, netbios_domain_and_sam_account_name, on_premise_security_identifier, sam_account_name, and use_guid.\nList of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim"

### fn spec.forProvider.optionalClaims.saml2Token.withAdditionalPropertiesMixin

```ts
withAdditionalPropertiesMixin(additionalProperties)
```

"List of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim. Possible values are: cloud_displayname, dns_domain_and_sam_account_name, emit_as_roles, include_externally_authenticated_upn_without_hash, include_externally_authenticated_upn, max_size_limit, netbios_domain_and_sam_account_name, on_premise_security_identifier, sam_account_name, and use_guid.\nList of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.optionalClaims.saml2Token.withEssential

```ts
withEssential(essential)
```

"Whether the claim specified by the client is necessary to ensure a smooth authorization experience.\nWhether the claim specified by the client is necessary to ensure a smooth authorization experience"

### fn spec.forProvider.optionalClaims.saml2Token.withName

```ts
withName(name)
```

"The name of the optional claim.\nThe name of the optional claim"

### fn spec.forProvider.optionalClaims.saml2Token.withSource

```ts
withSource(source)
```

"The source of the claim. If source is absent, the claim is a predefined optional claim. If source is user, the value of name is the extension property from the user object.\nThe source of the claim. If `source` is absent, the claim is a predefined optional claim. If `source` is `user`, the value of `name` is the extension property from the user object"

## obj spec.forProvider.password

"A single password block as documented below. The password is generated during creation. By default, no password is generated.\nApp password definition"

### fn spec.forProvider.password.withDisplayName

```ts
withDisplayName(displayName)
```

"A display name for the password. Changing this field forces a new resource to be created.\nA display name for the password"

### fn spec.forProvider.password.withEndDate

```ts
withEndDate(endDate)
```

"The end date until which the password is valid, formatted as an RFC3339 date string (e.g. 2018-01-01T01:02:03Z). Changing this field forces a new resource to be created.\nThe end date until which the password is valid, formatted as an RFC3339 date string (e.g. `2018-01-01T01:02:03Z`)"

### fn spec.forProvider.password.withStartDate

```ts
withStartDate(startDate)
```

"The start date from which the password is valid, formatted as an RFC3339 date string (e.g. 2018-01-01T01:02:03Z). If this isn't specified, the current date is used.  Changing this field forces a new resource to be created.\nThe start date from which the password is valid, formatted as an RFC3339 date string (e.g. `2018-01-01T01:02:03Z`). If this isn't specified, the current date is used"

## obj spec.forProvider.publicClient

"A public_client block as documented below, which configures non-web app or non-web API application settings, for example mobile or other public clients such as an installed application running on a desktop device."

### fn spec.forProvider.publicClient.withRedirectUris

```ts
withRedirectUris(redirectUris)
```

"A set of URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent. Must be a valid https or ms-appx-web URL.\nThe URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent"

### fn spec.forProvider.publicClient.withRedirectUrisMixin

```ts
withRedirectUrisMixin(redirectUris)
```

"A set of URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent. Must be a valid https or ms-appx-web URL.\nThe URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent"

**Note:** This function appends passed data to existing values

## obj spec.forProvider.requiredResourceAccess

"A collection of required_resource_access blocks as documented below."

### fn spec.forProvider.requiredResourceAccess.withResourceAccess

```ts
withResourceAccess(resourceAccess)
```

"A collection of resource_access blocks as documented below, describing OAuth2.0 permission scopes and app roles that the application requires from the specified resource."

### fn spec.forProvider.requiredResourceAccess.withResourceAccessMixin

```ts
withResourceAccessMixin(resourceAccess)
```

"A collection of resource_access blocks as documented below, describing OAuth2.0 permission scopes and app roles that the application requires from the specified resource."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.requiredResourceAccess.withResourceAppId

```ts
withResourceAppId(resourceAppId)
```

"The unique identifier for the resource that the application requires access to. This should be the Application ID of the target application."

## obj spec.forProvider.requiredResourceAccess.resourceAccess

"A collection of resource_access blocks as documented below, describing OAuth2.0 permission scopes and app roles that the application requires from the specified resource."

### fn spec.forProvider.requiredResourceAccess.resourceAccess.withId

```ts
withId(id)
```

"The unique identifier for an app role or OAuth2 permission scope published by the resource application."

### fn spec.forProvider.requiredResourceAccess.resourceAccess.withType

```ts
withType(type)
```

"Specifies whether the id property references an app role or an OAuth2 permission scope. Possible values are Role or Scope."

## obj spec.forProvider.singlePageApplication

"A single_page_application block as documented below, which configures single-page application (SPA) related settings for this application."

### fn spec.forProvider.singlePageApplication.withRedirectUris

```ts
withRedirectUris(redirectUris)
```

"A set of URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent. Must be a valid https URL.\nThe URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent"

### fn spec.forProvider.singlePageApplication.withRedirectUrisMixin

```ts
withRedirectUrisMixin(redirectUris)
```

"A set of URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent. Must be a valid https URL.\nThe URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent"

**Note:** This function appends passed data to existing values

## obj spec.forProvider.web

"A web block as documented below, which configures web related settings for this application."

### fn spec.forProvider.web.withHomepageUrl

```ts
withHomepageUrl(homepageUrl)
```

"Home page or landing page of the application.\nHome page or landing page of the application"

### fn spec.forProvider.web.withLogoutUrl

```ts
withLogoutUrl(logoutUrl)
```

"The URL that will be used by Microsoft's authorization service to sign out a user using front-channel, back-channel or SAML logout protocols.\nThe URL that will be used by Microsoft's authorization service to sign out a user using front-channel, back-channel or SAML logout protocols"

### fn spec.forProvider.web.withRedirectUris

```ts
withRedirectUris(redirectUris)
```

"A set of URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent. Must be a valid http URL or a URN.\nThe URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent"

### fn spec.forProvider.web.withRedirectUrisMixin

```ts
withRedirectUrisMixin(redirectUris)
```

"A set of URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent. Must be a valid http URL or a URN.\nThe URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent"

**Note:** This function appends passed data to existing values

## obj spec.forProvider.web.implicitGrant

"An implicit_grant block as documented above."

### fn spec.forProvider.web.implicitGrant.withAccessTokenIssuanceEnabled

```ts
withAccessTokenIssuanceEnabled(accessTokenIssuanceEnabled)
```

"Whether this web application can request an access token using OAuth 2.0 implicit flow.\nWhether this web application can request an access token using OAuth 2.0 implicit flow"

### fn spec.forProvider.web.implicitGrant.withIdTokenIssuanceEnabled

```ts
withIdTokenIssuanceEnabled(idTokenIssuanceEnabled)
```

"Whether this web application can request an ID token using OAuth 2.0 implicit flow.\nWhether this web application can request an ID token using OAuth 2.0 implicit flow"

## obj spec.initProvider

"THIS IS A BETA FIELD. It will be honored\nunless the Management Policies feature flag is disabled.\nInitProvider holds the same fields as ForProvider, with the exception\nof Identifier and other resource reference fields. The fields that are\nin InitProvider are merged into ForProvider when the resource is created.\nThe same fields are also added to the terraform ignore_changes hook, to\navoid updating them after creation. This is useful for fields that are\nrequired on creation, but we do not desire to update them after creation,\nfor example because of an external controller is managing them, like an\nautoscaler."

### fn spec.initProvider.withDescription

```ts
withDescription(description)
```

"A description of the application, as shown to end users.\nDescription of the application as shown to end users"

### fn spec.initProvider.withDeviceOnlyAuthEnabled

```ts
withDeviceOnlyAuthEnabled(deviceOnlyAuthEnabled)
```

"Specifies whether this application supports device authentication without a user. Defaults to false.\nSpecifies whether this application supports device authentication without a user."

### fn spec.initProvider.withDisplayName

```ts
withDisplayName(displayName)
```

"The display name for the application.\nThe display name for the application"

### fn spec.initProvider.withFallbackPublicClientEnabled

```ts
withFallbackPublicClientEnabled(fallbackPublicClientEnabled)
```

"Specifies whether the application is a public client. Appropriate for apps using token grant flows that don't use a redirect URI. Defaults to false.\nSpecifies whether the application is a public client. Appropriate for apps using token grant flows that don't use a redirect URI"

### fn spec.initProvider.withFeatureTags

```ts
withFeatureTags(featureTags)
```

"A feature_tags block as described below. Cannot be used together with the tags property.\nBlock of features to configure for this application using tags"

### fn spec.initProvider.withFeatureTagsMixin

```ts
withFeatureTagsMixin(featureTags)
```

"A feature_tags block as described below. Cannot be used together with the tags property.\nBlock of features to configure for this application using tags"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withGroupMembershipClaims

```ts
withGroupMembershipClaims(groupMembershipClaims)
```

"A set of strings containing membership claims issued in a user or OAuth 2.0 access token that the app expects. Possible values are None, SecurityGroup, DirectoryRole, ApplicationGroup or All.\nConfigures the `groups` claim issued in a user or OAuth 2.0 access token that the app expects"

### fn spec.initProvider.withGroupMembershipClaimsMixin

```ts
withGroupMembershipClaimsMixin(groupMembershipClaims)
```

"A set of strings containing membership claims issued in a user or OAuth 2.0 access token that the app expects. Possible values are None, SecurityGroup, DirectoryRole, ApplicationGroup or All.\nConfigures the `groups` claim issued in a user or OAuth 2.0 access token that the app expects"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withIdentifierUris

```ts
withIdentifierUris(identifierUris)
```

"A set of user-defined URI(s) that uniquely identify an application within its Azure AD tenant, or within a verified custom domain if the application is multi-tenant.\nThe user-defined URI(s) that uniquely identify an application within its Azure AD tenant, or within a verified custom domain if the application is multi-tenant"

### fn spec.initProvider.withIdentifierUrisMixin

```ts
withIdentifierUrisMixin(identifierUris)
```

"A set of user-defined URI(s) that uniquely identify an application within its Azure AD tenant, or within a verified custom domain if the application is multi-tenant.\nThe user-defined URI(s) that uniquely identify an application within its Azure AD tenant, or within a verified custom domain if the application is multi-tenant"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withLogoImage

```ts
withLogoImage(logoImage)
```

"A logo image to upload for the application, as a raw base64-encoded string. The image should be in gif, jpeg or png format. Note that once an image has been uploaded, it is not possible to remove it without replacing it with another image.\nBase64 encoded logo image in gif, png or jpeg format"

### fn spec.initProvider.withMarketingUrl

```ts
withMarketingUrl(marketingUrl)
```

"URL of the application's marketing page.\nURL of the application's marketing page"

### fn spec.initProvider.withNotes

```ts
withNotes(notes)
```

"User-specified notes relevant for the management of the application.\nUser-specified notes relevant for the management of the application"

### fn spec.initProvider.withOauth2PostResponseRequired

```ts
withOauth2PostResponseRequired(oauth2PostResponseRequired)
```

"Specifies whether, as part of OAuth 2.0 token requests, Azure AD allows POST requests, as opposed to GET requests. Defaults to false, which specifies that only GET requests are allowed.\nSpecifies whether, as part of OAuth 2.0 token requests, Azure AD allows POST requests, as opposed to GET requests."

### fn spec.initProvider.withOwners

```ts
withOwners(owners)
```

"A set of object IDs of principals that will be granted ownership of the application. Supported object types are users or service principals. By default, no owners are assigned.\nA list of object IDs of principals that will be granted ownership of the application"

### fn spec.initProvider.withOwnersMixin

```ts
withOwnersMixin(owners)
```

"A set of object IDs of principals that will be granted ownership of the application. Supported object types are users or service principals. By default, no owners are assigned.\nA list of object IDs of principals that will be granted ownership of the application"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withPreventDuplicateNames

```ts
withPreventDuplicateNames(preventDuplicateNames)
```

"If true, will return an error if an existing application is found with the same name. Defaults to false.\nIf `true`, will return an error if an existing application is found with the same name"

### fn spec.initProvider.withPrivacyStatementUrl

```ts
withPrivacyStatementUrl(privacyStatementUrl)
```

"URL of the application's privacy statement.\nURL of the application's privacy statement"

### fn spec.initProvider.withRequiredResourceAccess

```ts
withRequiredResourceAccess(requiredResourceAccess)
```

"A collection of required_resource_access blocks as documented below."

### fn spec.initProvider.withRequiredResourceAccessMixin

```ts
withRequiredResourceAccessMixin(requiredResourceAccess)
```

"A collection of required_resource_access blocks as documented below."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withServiceManagementReference

```ts
withServiceManagementReference(serviceManagementReference)
```

"References application context information from a Service or Asset Management database.\nReferences application or service contact information from a Service or Asset Management database"

### fn spec.initProvider.withSignInAudience

```ts
withSignInAudience(signInAudience)
```

"The Microsoft account types that are supported for the current application. Must be one of AzureADMyOrg, AzureADMultipleOrgs, AzureADandPersonalMicrosoftAccount or PersonalMicrosoftAccount. Defaults to AzureADMyOrg.\nThe Microsoft account types that are supported for the current application"

### fn spec.initProvider.withSupportUrl

```ts
withSupportUrl(supportUrl)
```

"URL of the application's support page.\nURL of the application's support page"

### fn spec.initProvider.withTags

```ts
withTags(tags)
```

"A set of tags to apply to the application for configuring specific behaviours of the application and linked service principals. Note that these are not provided for use by practitioners. Cannot be used together with the feature_tags block.\nA set of tags to apply to the application"

### fn spec.initProvider.withTagsMixin

```ts
withTagsMixin(tags)
```

"A set of tags to apply to the application for configuring specific behaviours of the application and linked service principals. Note that these are not provided for use by practitioners. Cannot be used together with the feature_tags block.\nA set of tags to apply to the application"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withTemplateId

```ts
withTemplateId(templateId)
```

"Unique ID for a templated application in the Azure AD App Gallery, from which to create the application. Changing this forces a new resource to be created.\nUnique ID of the application template from which this application is created"

### fn spec.initProvider.withTermsOfServiceUrl

```ts
withTermsOfServiceUrl(termsOfServiceUrl)
```

"URL of the application's terms of service statement.\nURL of the application's terms of service statement"

## obj spec.initProvider.api

"An api block as documented below, which configures API related settings for this application."

### fn spec.initProvider.api.withKnownClientApplications

```ts
withKnownClientApplications(knownClientApplications)
```

"A set of client IDs, used for bundling consent if you have a solution that contains two parts: a client app and a custom web API app.\nUsed for bundling consent if you have a solution that contains two parts: a client app and a custom web API app"

### fn spec.initProvider.api.withKnownClientApplicationsMixin

```ts
withKnownClientApplicationsMixin(knownClientApplications)
```

"A set of client IDs, used for bundling consent if you have a solution that contains two parts: a client app and a custom web API app.\nUsed for bundling consent if you have a solution that contains two parts: a client app and a custom web API app"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.api.withKnownClientApplicationsRefs

```ts
withKnownClientApplicationsRefs(knownClientApplicationsRefs)
```

"References to Application in applications to populate knownClientApplications."

### fn spec.initProvider.api.withKnownClientApplicationsRefsMixin

```ts
withKnownClientApplicationsRefsMixin(knownClientApplicationsRefs)
```

"References to Application in applications to populate knownClientApplications."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.api.withMappedClaimsEnabled

```ts
withMappedClaimsEnabled(mappedClaimsEnabled)
```

"Allows an application to use claims mapping without specifying a custom signing key. Defaults to false.\nAllows an application to use claims mapping without specifying a custom signing key"

### fn spec.initProvider.api.withOauth2PermissionScope

```ts
withOauth2PermissionScope(oauth2PermissionScope)
```

"One or more oauth2_permission_scope blocks as documented below, to describe delegated permissions exposed by the web API represented by this application.\nOne or more `oauth2_permission_scope` blocks to describe delegated permissions exposed by the web API represented by this application"

### fn spec.initProvider.api.withOauth2PermissionScopeMixin

```ts
withOauth2PermissionScopeMixin(oauth2PermissionScope)
```

"One or more oauth2_permission_scope blocks as documented below, to describe delegated permissions exposed by the web API represented by this application.\nOne or more `oauth2_permission_scope` blocks to describe delegated permissions exposed by the web API represented by this application"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.api.withRequestedAccessTokenVersion

```ts
withRequestedAccessTokenVersion(requestedAccessTokenVersion)
```

"The access token version expected by this resource. Must be one of 1 or 2, and must be 2 when sign_in_audience is either AzureADandPersonalMicrosoftAccount or PersonalMicrosoftAccount Defaults to 1.\nThe access token version expected by this resource"

## obj spec.initProvider.api.knownClientApplicationsRefs

"References to Application in applications to populate knownClientApplications."

### fn spec.initProvider.api.knownClientApplicationsRefs.withName

```ts
withName(name)
```

"Name of the referenced object."

## obj spec.initProvider.api.knownClientApplicationsRefs.policy

"Policies for referencing."

### fn spec.initProvider.api.knownClientApplicationsRefs.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.initProvider.api.knownClientApplicationsRefs.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.initProvider.api.knownClientApplicationsSelector

"Selector for a list of Application in applications to populate knownClientApplications."

### fn spec.initProvider.api.knownClientApplicationsSelector.withMatchControllerRef

```ts
withMatchControllerRef(matchControllerRef)
```

"MatchControllerRef ensures an object with the same controller reference\nas the selecting object is selected."

### fn spec.initProvider.api.knownClientApplicationsSelector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

### fn spec.initProvider.api.knownClientApplicationsSelector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"MatchLabels ensures an object with matching labels is selected."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.api.knownClientApplicationsSelector.policy

"Policies for selection."

### fn spec.initProvider.api.knownClientApplicationsSelector.policy.withResolution

```ts
withResolution(resolution)
```

"Resolution specifies whether resolution of this reference is required.\nThe default is 'Required', which means the reconcile will fail if the\nreference cannot be resolved. 'Optional' means this reference will be\na no-op if it cannot be resolved."

### fn spec.initProvider.api.knownClientApplicationsSelector.policy.withResolve

```ts
withResolve(resolve)
```

"Resolve specifies when this reference should be resolved. The default\nis 'IfNotPresent', which will attempt to resolve the reference only when\nthe corresponding field is not present. Use 'Always' to resolve the\nreference on every reconcile."

## obj spec.initProvider.api.oauth2PermissionScope

"One or more oauth2_permission_scope blocks as documented below, to describe delegated permissions exposed by the web API represented by this application.\nOne or more `oauth2_permission_scope` blocks to describe delegated permissions exposed by the web API represented by this application"

### fn spec.initProvider.api.oauth2PermissionScope.withAdminConsentDescription

```ts
withAdminConsentDescription(adminConsentDescription)
```

"Delegated permission description that appears in all tenant-wide admin consent experiences, intended to be read by an administrator granting the permission on behalf of all users.\nDelegated permission description that appears in all tenant-wide admin consent experiences, intended to be read by an administrator granting the permission on behalf of all users"

### fn spec.initProvider.api.oauth2PermissionScope.withAdminConsentDisplayName

```ts
withAdminConsentDisplayName(adminConsentDisplayName)
```

"Display name for the delegated permission, intended to be read by an administrator granting the permission on behalf of all users.\nDisplay name for the delegated permission, intended to be read by an administrator granting the permission on behalf of all users"

### fn spec.initProvider.api.oauth2PermissionScope.withEnabled

```ts
withEnabled(enabled)
```

"Determines if the permission scope is enabled. Defaults to true.\nDetermines if the permission scope is enabled"

### fn spec.initProvider.api.oauth2PermissionScope.withId

```ts
withId(id)
```

"The unique identifier of the delegated permission. Must be a valid UUID.\nThe unique identifier of the delegated permission"

### fn spec.initProvider.api.oauth2PermissionScope.withType

```ts
withType(type)
```

"Whether this delegated permission should be considered safe for non-admin users to consent to on behalf of themselves, or whether an administrator should be required for consent to the permissions. Defaults to User. Possible values are User or Admin.\nWhether this delegated permission should be considered safe for non-admin users to consent to on behalf of themselves, or whether an administrator should be required for consent to the permissions"

### fn spec.initProvider.api.oauth2PermissionScope.withUserConsentDescription

```ts
withUserConsentDescription(userConsentDescription)
```

"Delegated permission description that appears in the end user consent experience, intended to be read by a user consenting on their own behalf.\nDelegated permission description that appears in the end user consent experience, intended to be read by a user consenting on their own behalf"

### fn spec.initProvider.api.oauth2PermissionScope.withUserConsentDisplayName

```ts
withUserConsentDisplayName(userConsentDisplayName)
```

"Display name for the delegated permission that appears in the end user consent experience.\nDisplay name for the delegated permission that appears in the end user consent experience"

### fn spec.initProvider.api.oauth2PermissionScope.withValue

```ts
withValue(value)
```

"The value that is used for the scp claim in OAuth 2.0 access tokens.\nThe value that is used for the `scp` claim in OAuth 2.0 access tokens"

## obj spec.initProvider.featureTags

"A feature_tags block as described below. Cannot be used together with the tags property.\nBlock of features to configure for this application using tags"

### fn spec.initProvider.featureTags.withCustomSingleSignOn

```ts
withCustomSingleSignOn(customSingleSignOn)
```

"Whether this application represents a custom SAML application for linked service principals. Enabling this will assign the WindowsAzureActiveDirectoryCustomSingleSignOnApplication tag. Defaults to false.\nWhether this application represents a custom SAML application for linked service principals"

### fn spec.initProvider.featureTags.withEnterprise

```ts
withEnterprise(enterprise)
```

"Whether this application represents an Enterprise Application for linked service principals. Enabling this will assign the WindowsAzureActiveDirectoryIntegratedApp tag. Defaults to false.\nWhether this application represents an Enterprise Application for linked service principals"

### fn spec.initProvider.featureTags.withGallery

```ts
withGallery(gallery)
```

"Whether this application represents a gallery application for linked service principals. Enabling this will assign the WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1 tag. Defaults to false.\nWhether this application represents a gallery application for linked service principals"

### fn spec.initProvider.featureTags.withHide

```ts
withHide(hide)
```

"Whether this app is invisible to users in My Apps and Office 365 Launcher. Enabling this will assign the HideApp tag. Defaults to false.\nWhether this application is invisible to users in My Apps and Office 365 Launcher"

## obj spec.initProvider.optionalClaims

"An optional_claims block as documented below."

### fn spec.initProvider.optionalClaims.withAccessToken

```ts
withAccessToken(accessToken)
```

"One or more access_token blocks as documented below."

### fn spec.initProvider.optionalClaims.withAccessTokenMixin

```ts
withAccessTokenMixin(accessToken)
```

"One or more access_token blocks as documented below."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.optionalClaims.withIdToken

```ts
withIdToken(idToken)
```

"One or more id_token blocks as documented below."

### fn spec.initProvider.optionalClaims.withIdTokenMixin

```ts
withIdTokenMixin(idToken)
```

"One or more id_token blocks as documented below."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.optionalClaims.withSaml2Token

```ts
withSaml2Token(saml2Token)
```

"One or more saml2_token blocks as documented below."

### fn spec.initProvider.optionalClaims.withSaml2TokenMixin

```ts
withSaml2TokenMixin(saml2Token)
```

"One or more saml2_token blocks as documented below."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.optionalClaims.accessToken

"One or more access_token blocks as documented below."

### fn spec.initProvider.optionalClaims.accessToken.withAdditionalProperties

```ts
withAdditionalProperties(additionalProperties)
```

"List of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim. Possible values are: cloud_displayname, dns_domain_and_sam_account_name, emit_as_roles, include_externally_authenticated_upn_without_hash, include_externally_authenticated_upn, max_size_limit, netbios_domain_and_sam_account_name, on_premise_security_identifier, sam_account_name, and use_guid.\nList of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim"

### fn spec.initProvider.optionalClaims.accessToken.withAdditionalPropertiesMixin

```ts
withAdditionalPropertiesMixin(additionalProperties)
```

"List of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim. Possible values are: cloud_displayname, dns_domain_and_sam_account_name, emit_as_roles, include_externally_authenticated_upn_without_hash, include_externally_authenticated_upn, max_size_limit, netbios_domain_and_sam_account_name, on_premise_security_identifier, sam_account_name, and use_guid.\nList of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.optionalClaims.accessToken.withEssential

```ts
withEssential(essential)
```

"Whether the claim specified by the client is necessary to ensure a smooth authorization experience.\nWhether the claim specified by the client is necessary to ensure a smooth authorization experience"

### fn spec.initProvider.optionalClaims.accessToken.withName

```ts
withName(name)
```

"The name of the optional claim.\nThe name of the optional claim"

### fn spec.initProvider.optionalClaims.accessToken.withSource

```ts
withSource(source)
```

"The source of the claim. If source is absent, the claim is a predefined optional claim. If source is user, the value of name is the extension property from the user object.\nThe source of the claim. If `source` is absent, the claim is a predefined optional claim. If `source` is `user`, the value of `name` is the extension property from the user object"

## obj spec.initProvider.optionalClaims.idToken

"One or more id_token blocks as documented below."

### fn spec.initProvider.optionalClaims.idToken.withAdditionalProperties

```ts
withAdditionalProperties(additionalProperties)
```

"List of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim. Possible values are: cloud_displayname, dns_domain_and_sam_account_name, emit_as_roles, include_externally_authenticated_upn_without_hash, include_externally_authenticated_upn, max_size_limit, netbios_domain_and_sam_account_name, on_premise_security_identifier, sam_account_name, and use_guid.\nList of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim"

### fn spec.initProvider.optionalClaims.idToken.withAdditionalPropertiesMixin

```ts
withAdditionalPropertiesMixin(additionalProperties)
```

"List of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim. Possible values are: cloud_displayname, dns_domain_and_sam_account_name, emit_as_roles, include_externally_authenticated_upn_without_hash, include_externally_authenticated_upn, max_size_limit, netbios_domain_and_sam_account_name, on_premise_security_identifier, sam_account_name, and use_guid.\nList of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.optionalClaims.idToken.withEssential

```ts
withEssential(essential)
```

"Whether the claim specified by the client is necessary to ensure a smooth authorization experience.\nWhether the claim specified by the client is necessary to ensure a smooth authorization experience"

### fn spec.initProvider.optionalClaims.idToken.withName

```ts
withName(name)
```

"The name of the optional claim.\nThe name of the optional claim"

### fn spec.initProvider.optionalClaims.idToken.withSource

```ts
withSource(source)
```

"The source of the claim. If source is absent, the claim is a predefined optional claim. If source is user, the value of name is the extension property from the user object.\nThe source of the claim. If `source` is absent, the claim is a predefined optional claim. If `source` is `user`, the value of `name` is the extension property from the user object"

## obj spec.initProvider.optionalClaims.saml2Token

"One or more saml2_token blocks as documented below."

### fn spec.initProvider.optionalClaims.saml2Token.withAdditionalProperties

```ts
withAdditionalProperties(additionalProperties)
```

"List of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim. Possible values are: cloud_displayname, dns_domain_and_sam_account_name, emit_as_roles, include_externally_authenticated_upn_without_hash, include_externally_authenticated_upn, max_size_limit, netbios_domain_and_sam_account_name, on_premise_security_identifier, sam_account_name, and use_guid.\nList of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim"

### fn spec.initProvider.optionalClaims.saml2Token.withAdditionalPropertiesMixin

```ts
withAdditionalPropertiesMixin(additionalProperties)
```

"List of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim. Possible values are: cloud_displayname, dns_domain_and_sam_account_name, emit_as_roles, include_externally_authenticated_upn_without_hash, include_externally_authenticated_upn, max_size_limit, netbios_domain_and_sam_account_name, on_premise_security_identifier, sam_account_name, and use_guid.\nList of additional properties of the claim. If a property exists in this list, it modifies the behaviour of the optional claim"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.optionalClaims.saml2Token.withEssential

```ts
withEssential(essential)
```

"Whether the claim specified by the client is necessary to ensure a smooth authorization experience.\nWhether the claim specified by the client is necessary to ensure a smooth authorization experience"

### fn spec.initProvider.optionalClaims.saml2Token.withName

```ts
withName(name)
```

"The name of the optional claim.\nThe name of the optional claim"

### fn spec.initProvider.optionalClaims.saml2Token.withSource

```ts
withSource(source)
```

"The source of the claim. If source is absent, the claim is a predefined optional claim. If source is user, the value of name is the extension property from the user object.\nThe source of the claim. If `source` is absent, the claim is a predefined optional claim. If `source` is `user`, the value of `name` is the extension property from the user object"

## obj spec.initProvider.password

"A single password block as documented below. The password is generated during creation. By default, no password is generated.\nApp password definition"

### fn spec.initProvider.password.withDisplayName

```ts
withDisplayName(displayName)
```

"A display name for the password. Changing this field forces a new resource to be created.\nA display name for the password"

### fn spec.initProvider.password.withEndDate

```ts
withEndDate(endDate)
```

"The end date until which the password is valid, formatted as an RFC3339 date string (e.g. 2018-01-01T01:02:03Z). Changing this field forces a new resource to be created.\nThe end date until which the password is valid, formatted as an RFC3339 date string (e.g. `2018-01-01T01:02:03Z`)"

### fn spec.initProvider.password.withStartDate

```ts
withStartDate(startDate)
```

"The start date from which the password is valid, formatted as an RFC3339 date string (e.g. 2018-01-01T01:02:03Z). If this isn't specified, the current date is used.  Changing this field forces a new resource to be created.\nThe start date from which the password is valid, formatted as an RFC3339 date string (e.g. `2018-01-01T01:02:03Z`). If this isn't specified, the current date is used"

## obj spec.initProvider.publicClient

"A public_client block as documented below, which configures non-web app or non-web API application settings, for example mobile or other public clients such as an installed application running on a desktop device."

### fn spec.initProvider.publicClient.withRedirectUris

```ts
withRedirectUris(redirectUris)
```

"A set of URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent. Must be a valid https or ms-appx-web URL.\nThe URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent"

### fn spec.initProvider.publicClient.withRedirectUrisMixin

```ts
withRedirectUrisMixin(redirectUris)
```

"A set of URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent. Must be a valid https or ms-appx-web URL.\nThe URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent"

**Note:** This function appends passed data to existing values

## obj spec.initProvider.requiredResourceAccess

"A collection of required_resource_access blocks as documented below."

### fn spec.initProvider.requiredResourceAccess.withResourceAccess

```ts
withResourceAccess(resourceAccess)
```

"A collection of resource_access blocks as documented below, describing OAuth2.0 permission scopes and app roles that the application requires from the specified resource."

### fn spec.initProvider.requiredResourceAccess.withResourceAccessMixin

```ts
withResourceAccessMixin(resourceAccess)
```

"A collection of resource_access blocks as documented below, describing OAuth2.0 permission scopes and app roles that the application requires from the specified resource."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.requiredResourceAccess.withResourceAppId

```ts
withResourceAppId(resourceAppId)
```

"The unique identifier for the resource that the application requires access to. This should be the Application ID of the target application."

## obj spec.initProvider.requiredResourceAccess.resourceAccess

"A collection of resource_access blocks as documented below, describing OAuth2.0 permission scopes and app roles that the application requires from the specified resource."

### fn spec.initProvider.requiredResourceAccess.resourceAccess.withId

```ts
withId(id)
```

"The unique identifier for an app role or OAuth2 permission scope published by the resource application."

### fn spec.initProvider.requiredResourceAccess.resourceAccess.withType

```ts
withType(type)
```

"Specifies whether the id property references an app role or an OAuth2 permission scope. Possible values are Role or Scope."

## obj spec.initProvider.singlePageApplication

"A single_page_application block as documented below, which configures single-page application (SPA) related settings for this application."

### fn spec.initProvider.singlePageApplication.withRedirectUris

```ts
withRedirectUris(redirectUris)
```

"A set of URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent. Must be a valid https URL.\nThe URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent"

### fn spec.initProvider.singlePageApplication.withRedirectUrisMixin

```ts
withRedirectUrisMixin(redirectUris)
```

"A set of URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent. Must be a valid https URL.\nThe URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent"

**Note:** This function appends passed data to existing values

## obj spec.initProvider.web

"A web block as documented below, which configures web related settings for this application."

### fn spec.initProvider.web.withHomepageUrl

```ts
withHomepageUrl(homepageUrl)
```

"Home page or landing page of the application.\nHome page or landing page of the application"

### fn spec.initProvider.web.withLogoutUrl

```ts
withLogoutUrl(logoutUrl)
```

"The URL that will be used by Microsoft's authorization service to sign out a user using front-channel, back-channel or SAML logout protocols.\nThe URL that will be used by Microsoft's authorization service to sign out a user using front-channel, back-channel or SAML logout protocols"

### fn spec.initProvider.web.withRedirectUris

```ts
withRedirectUris(redirectUris)
```

"A set of URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent. Must be a valid http URL or a URN.\nThe URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent"

### fn spec.initProvider.web.withRedirectUrisMixin

```ts
withRedirectUrisMixin(redirectUris)
```

"A set of URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent. Must be a valid http URL or a URN.\nThe URLs where user tokens are sent for sign-in, or the redirect URIs where OAuth 2.0 authorization codes and access tokens are sent"

**Note:** This function appends passed data to existing values

## obj spec.initProvider.web.implicitGrant

"An implicit_grant block as documented above."

### fn spec.initProvider.web.implicitGrant.withAccessTokenIssuanceEnabled

```ts
withAccessTokenIssuanceEnabled(accessTokenIssuanceEnabled)
```

"Whether this web application can request an access token using OAuth 2.0 implicit flow.\nWhether this web application can request an access token using OAuth 2.0 implicit flow"

### fn spec.initProvider.web.implicitGrant.withIdTokenIssuanceEnabled

```ts
withIdTokenIssuanceEnabled(idTokenIssuanceEnabled)
```

"Whether this web application can request an ID token using OAuth 2.0 implicit flow.\nWhether this web application can request an ID token using OAuth 2.0 implicit flow"

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