---
permalink: /upbound-provider-azuread/cluster/conditionalaccess/v1beta1/accessPolicy/
---

# conditionalaccess.v1beta1.accessPolicy

"AccessPolicy is the Schema for the AccessPolicys API."

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
    * [`fn withConditions(conditions)`](#fn-specforproviderwithconditions)
    * [`fn withConditionsMixin(conditions)`](#fn-specforproviderwithconditionsmixin)
    * [`fn withDisplayName(displayName)`](#fn-specforproviderwithdisplayname)
    * [`fn withGrantControls(grantControls)`](#fn-specforproviderwithgrantcontrols)
    * [`fn withGrantControlsMixin(grantControls)`](#fn-specforproviderwithgrantcontrolsmixin)
    * [`fn withSessionControls(sessionControls)`](#fn-specforproviderwithsessioncontrols)
    * [`fn withSessionControlsMixin(sessionControls)`](#fn-specforproviderwithsessioncontrolsmixin)
    * [`fn withState(state)`](#fn-specforproviderwithstate)
    * [`obj spec.forProvider.conditions`](#obj-specforproviderconditions)
      * [`fn withApplications(applications)`](#fn-specforproviderconditionswithapplications)
      * [`fn withApplicationsMixin(applications)`](#fn-specforproviderconditionswithapplicationsmixin)
      * [`fn withClientAppTypes(clientAppTypes)`](#fn-specforproviderconditionswithclientapptypes)
      * [`fn withClientAppTypesMixin(clientAppTypes)`](#fn-specforproviderconditionswithclientapptypesmixin)
      * [`fn withClientApplications(clientApplications)`](#fn-specforproviderconditionswithclientapplications)
      * [`fn withClientApplicationsMixin(clientApplications)`](#fn-specforproviderconditionswithclientapplicationsmixin)
      * [`fn withDevices(devices)`](#fn-specforproviderconditionswithdevices)
      * [`fn withDevicesMixin(devices)`](#fn-specforproviderconditionswithdevicesmixin)
      * [`fn withInsiderRiskLevels(insiderRiskLevels)`](#fn-specforproviderconditionswithinsiderrisklevels)
      * [`fn withLocations(locations)`](#fn-specforproviderconditionswithlocations)
      * [`fn withLocationsMixin(locations)`](#fn-specforproviderconditionswithlocationsmixin)
      * [`fn withPlatforms(platforms)`](#fn-specforproviderconditionswithplatforms)
      * [`fn withPlatformsMixin(platforms)`](#fn-specforproviderconditionswithplatformsmixin)
      * [`fn withServicePrincipalRiskLevels(servicePrincipalRiskLevels)`](#fn-specforproviderconditionswithserviceprincipalrisklevels)
      * [`fn withServicePrincipalRiskLevelsMixin(servicePrincipalRiskLevels)`](#fn-specforproviderconditionswithserviceprincipalrisklevelsmixin)
      * [`fn withSignInRiskLevels(signInRiskLevels)`](#fn-specforproviderconditionswithsigninrisklevels)
      * [`fn withSignInRiskLevelsMixin(signInRiskLevels)`](#fn-specforproviderconditionswithsigninrisklevelsmixin)
      * [`fn withUserRiskLevels(userRiskLevels)`](#fn-specforproviderconditionswithuserrisklevels)
      * [`fn withUserRiskLevelsMixin(userRiskLevels)`](#fn-specforproviderconditionswithuserrisklevelsmixin)
      * [`fn withUsers(users)`](#fn-specforproviderconditionswithusers)
      * [`fn withUsersMixin(users)`](#fn-specforproviderconditionswithusersmixin)
      * [`obj spec.forProvider.conditions.applications`](#obj-specforproviderconditionsapplications)
        * [`fn withExcludedApplications(excludedApplications)`](#fn-specforproviderconditionsapplicationswithexcludedapplications)
        * [`fn withExcludedApplicationsMixin(excludedApplications)`](#fn-specforproviderconditionsapplicationswithexcludedapplicationsmixin)
        * [`fn withIncludedApplications(includedApplications)`](#fn-specforproviderconditionsapplicationswithincludedapplications)
        * [`fn withIncludedApplicationsMixin(includedApplications)`](#fn-specforproviderconditionsapplicationswithincludedapplicationsmixin)
        * [`fn withIncludedUserActions(includedUserActions)`](#fn-specforproviderconditionsapplicationswithincludeduseractions)
        * [`fn withIncludedUserActionsMixin(includedUserActions)`](#fn-specforproviderconditionsapplicationswithincludeduseractionsmixin)
      * [`obj spec.forProvider.conditions.clientApplications`](#obj-specforproviderconditionsclientapplications)
        * [`fn withExcludedServicePrincipals(excludedServicePrincipals)`](#fn-specforproviderconditionsclientapplicationswithexcludedserviceprincipals)
        * [`fn withExcludedServicePrincipalsMixin(excludedServicePrincipals)`](#fn-specforproviderconditionsclientapplicationswithexcludedserviceprincipalsmixin)
        * [`fn withIncludedServicePrincipals(includedServicePrincipals)`](#fn-specforproviderconditionsclientapplicationswithincludedserviceprincipals)
        * [`fn withIncludedServicePrincipalsMixin(includedServicePrincipals)`](#fn-specforproviderconditionsclientapplicationswithincludedserviceprincipalsmixin)
      * [`obj spec.forProvider.conditions.devices`](#obj-specforproviderconditionsdevices)
        * [`fn withFilter(filter)`](#fn-specforproviderconditionsdeviceswithfilter)
        * [`fn withFilterMixin(filter)`](#fn-specforproviderconditionsdeviceswithfiltermixin)
        * [`obj spec.forProvider.conditions.devices.filter`](#obj-specforproviderconditionsdevicesfilter)
          * [`fn withMode(mode)`](#fn-specforproviderconditionsdevicesfilterwithmode)
          * [`fn withRule(rule)`](#fn-specforproviderconditionsdevicesfilterwithrule)
      * [`obj spec.forProvider.conditions.locations`](#obj-specforproviderconditionslocations)
        * [`fn withExcludedLocations(excludedLocations)`](#fn-specforproviderconditionslocationswithexcludedlocations)
        * [`fn withExcludedLocationsMixin(excludedLocations)`](#fn-specforproviderconditionslocationswithexcludedlocationsmixin)
        * [`fn withIncludedLocations(includedLocations)`](#fn-specforproviderconditionslocationswithincludedlocations)
        * [`fn withIncludedLocationsMixin(includedLocations)`](#fn-specforproviderconditionslocationswithincludedlocationsmixin)
      * [`obj spec.forProvider.conditions.platforms`](#obj-specforproviderconditionsplatforms)
        * [`fn withExcludedPlatforms(excludedPlatforms)`](#fn-specforproviderconditionsplatformswithexcludedplatforms)
        * [`fn withExcludedPlatformsMixin(excludedPlatforms)`](#fn-specforproviderconditionsplatformswithexcludedplatformsmixin)
        * [`fn withIncludedPlatforms(includedPlatforms)`](#fn-specforproviderconditionsplatformswithincludedplatforms)
        * [`fn withIncludedPlatformsMixin(includedPlatforms)`](#fn-specforproviderconditionsplatformswithincludedplatformsmixin)
      * [`obj spec.forProvider.conditions.users`](#obj-specforproviderconditionsusers)
        * [`fn withExcludedGroups(excludedGroups)`](#fn-specforproviderconditionsuserswithexcludedgroups)
        * [`fn withExcludedGroupsMixin(excludedGroups)`](#fn-specforproviderconditionsuserswithexcludedgroupsmixin)
        * [`fn withExcludedGuestsOrExternalUsers(excludedGuestsOrExternalUsers)`](#fn-specforproviderconditionsuserswithexcludedguestsorexternalusers)
        * [`fn withExcludedGuestsOrExternalUsersMixin(excludedGuestsOrExternalUsers)`](#fn-specforproviderconditionsuserswithexcludedguestsorexternalusersmixin)
        * [`fn withExcludedRoles(excludedRoles)`](#fn-specforproviderconditionsuserswithexcludedroles)
        * [`fn withExcludedRolesMixin(excludedRoles)`](#fn-specforproviderconditionsuserswithexcludedrolesmixin)
        * [`fn withExcludedUsers(excludedUsers)`](#fn-specforproviderconditionsuserswithexcludedusers)
        * [`fn withExcludedUsersMixin(excludedUsers)`](#fn-specforproviderconditionsuserswithexcludedusersmixin)
        * [`fn withIncludedGroups(includedGroups)`](#fn-specforproviderconditionsuserswithincludedgroups)
        * [`fn withIncludedGroupsMixin(includedGroups)`](#fn-specforproviderconditionsuserswithincludedgroupsmixin)
        * [`fn withIncludedGuestsOrExternalUsers(includedGuestsOrExternalUsers)`](#fn-specforproviderconditionsuserswithincludedguestsorexternalusers)
        * [`fn withIncludedGuestsOrExternalUsersMixin(includedGuestsOrExternalUsers)`](#fn-specforproviderconditionsuserswithincludedguestsorexternalusersmixin)
        * [`fn withIncludedRoles(includedRoles)`](#fn-specforproviderconditionsuserswithincludedroles)
        * [`fn withIncludedRolesMixin(includedRoles)`](#fn-specforproviderconditionsuserswithincludedrolesmixin)
        * [`fn withIncludedUsers(includedUsers)`](#fn-specforproviderconditionsuserswithincludedusers)
        * [`fn withIncludedUsersMixin(includedUsers)`](#fn-specforproviderconditionsuserswithincludedusersmixin)
        * [`obj spec.forProvider.conditions.users.excludedGuestsOrExternalUsers`](#obj-specforproviderconditionsusersexcludedguestsorexternalusers)
          * [`fn withExternalTenants(externalTenants)`](#fn-specforproviderconditionsusersexcludedguestsorexternaluserswithexternaltenants)
          * [`fn withExternalTenantsMixin(externalTenants)`](#fn-specforproviderconditionsusersexcludedguestsorexternaluserswithexternaltenantsmixin)
          * [`fn withGuestOrExternalUserTypes(guestOrExternalUserTypes)`](#fn-specforproviderconditionsusersexcludedguestsorexternaluserswithguestorexternalusertypes)
          * [`fn withGuestOrExternalUserTypesMixin(guestOrExternalUserTypes)`](#fn-specforproviderconditionsusersexcludedguestsorexternaluserswithguestorexternalusertypesmixin)
          * [`obj spec.forProvider.conditions.users.excludedGuestsOrExternalUsers.externalTenants`](#obj-specforproviderconditionsusersexcludedguestsorexternalusersexternaltenants)
            * [`fn withMembers(members)`](#fn-specforproviderconditionsusersexcludedguestsorexternalusersexternaltenantswithmembers)
            * [`fn withMembersMixin(members)`](#fn-specforproviderconditionsusersexcludedguestsorexternalusersexternaltenantswithmembersmixin)
            * [`fn withMembershipKind(membershipKind)`](#fn-specforproviderconditionsusersexcludedguestsorexternalusersexternaltenantswithmembershipkind)
        * [`obj spec.forProvider.conditions.users.includedGuestsOrExternalUsers`](#obj-specforproviderconditionsusersincludedguestsorexternalusers)
          * [`fn withExternalTenants(externalTenants)`](#fn-specforproviderconditionsusersincludedguestsorexternaluserswithexternaltenants)
          * [`fn withExternalTenantsMixin(externalTenants)`](#fn-specforproviderconditionsusersincludedguestsorexternaluserswithexternaltenantsmixin)
          * [`fn withGuestOrExternalUserTypes(guestOrExternalUserTypes)`](#fn-specforproviderconditionsusersincludedguestsorexternaluserswithguestorexternalusertypes)
          * [`fn withGuestOrExternalUserTypesMixin(guestOrExternalUserTypes)`](#fn-specforproviderconditionsusersincludedguestsorexternaluserswithguestorexternalusertypesmixin)
          * [`obj spec.forProvider.conditions.users.includedGuestsOrExternalUsers.externalTenants`](#obj-specforproviderconditionsusersincludedguestsorexternalusersexternaltenants)
            * [`fn withMembers(members)`](#fn-specforproviderconditionsusersincludedguestsorexternalusersexternaltenantswithmembers)
            * [`fn withMembersMixin(members)`](#fn-specforproviderconditionsusersincludedguestsorexternalusersexternaltenantswithmembersmixin)
            * [`fn withMembershipKind(membershipKind)`](#fn-specforproviderconditionsusersincludedguestsorexternalusersexternaltenantswithmembershipkind)
    * [`obj spec.forProvider.grantControls`](#obj-specforprovidergrantcontrols)
      * [`fn withAuthenticationStrengthPolicyId(authenticationStrengthPolicyId)`](#fn-specforprovidergrantcontrolswithauthenticationstrengthpolicyid)
      * [`fn withBuiltInControls(builtInControls)`](#fn-specforprovidergrantcontrolswithbuiltincontrols)
      * [`fn withBuiltInControlsMixin(builtInControls)`](#fn-specforprovidergrantcontrolswithbuiltincontrolsmixin)
      * [`fn withCustomAuthenticationFactors(customAuthenticationFactors)`](#fn-specforprovidergrantcontrolswithcustomauthenticationfactors)
      * [`fn withCustomAuthenticationFactorsMixin(customAuthenticationFactors)`](#fn-specforprovidergrantcontrolswithcustomauthenticationfactorsmixin)
      * [`fn withOperator(operator)`](#fn-specforprovidergrantcontrolswithoperator)
      * [`fn withTermsOfUse(termsOfUse)`](#fn-specforprovidergrantcontrolswithtermsofuse)
      * [`fn withTermsOfUseMixin(termsOfUse)`](#fn-specforprovidergrantcontrolswithtermsofusemixin)
    * [`obj spec.forProvider.sessionControls`](#obj-specforprovidersessioncontrols)
      * [`fn withApplicationEnforcedRestrictionsEnabled(applicationEnforcedRestrictionsEnabled)`](#fn-specforprovidersessioncontrolswithapplicationenforcedrestrictionsenabled)
      * [`fn withCloudAppSecurityPolicy(cloudAppSecurityPolicy)`](#fn-specforprovidersessioncontrolswithcloudappsecuritypolicy)
      * [`fn withDisableResilienceDefaults(disableResilienceDefaults)`](#fn-specforprovidersessioncontrolswithdisableresiliencedefaults)
      * [`fn withPersistentBrowserMode(persistentBrowserMode)`](#fn-specforprovidersessioncontrolswithpersistentbrowsermode)
      * [`fn withSignInFrequency(signInFrequency)`](#fn-specforprovidersessioncontrolswithsigninfrequency)
      * [`fn withSignInFrequencyAuthenticationType(signInFrequencyAuthenticationType)`](#fn-specforprovidersessioncontrolswithsigninfrequencyauthenticationtype)
      * [`fn withSignInFrequencyInterval(signInFrequencyInterval)`](#fn-specforprovidersessioncontrolswithsigninfrequencyinterval)
      * [`fn withSignInFrequencyPeriod(signInFrequencyPeriod)`](#fn-specforprovidersessioncontrolswithsigninfrequencyperiod)
  * [`obj spec.initProvider`](#obj-specinitprovider)
    * [`fn withConditions(conditions)`](#fn-specinitproviderwithconditions)
    * [`fn withConditionsMixin(conditions)`](#fn-specinitproviderwithconditionsmixin)
    * [`fn withDisplayName(displayName)`](#fn-specinitproviderwithdisplayname)
    * [`fn withGrantControls(grantControls)`](#fn-specinitproviderwithgrantcontrols)
    * [`fn withGrantControlsMixin(grantControls)`](#fn-specinitproviderwithgrantcontrolsmixin)
    * [`fn withSessionControls(sessionControls)`](#fn-specinitproviderwithsessioncontrols)
    * [`fn withSessionControlsMixin(sessionControls)`](#fn-specinitproviderwithsessioncontrolsmixin)
    * [`fn withState(state)`](#fn-specinitproviderwithstate)
    * [`obj spec.initProvider.conditions`](#obj-specinitproviderconditions)
      * [`fn withApplications(applications)`](#fn-specinitproviderconditionswithapplications)
      * [`fn withApplicationsMixin(applications)`](#fn-specinitproviderconditionswithapplicationsmixin)
      * [`fn withClientAppTypes(clientAppTypes)`](#fn-specinitproviderconditionswithclientapptypes)
      * [`fn withClientAppTypesMixin(clientAppTypes)`](#fn-specinitproviderconditionswithclientapptypesmixin)
      * [`fn withClientApplications(clientApplications)`](#fn-specinitproviderconditionswithclientapplications)
      * [`fn withClientApplicationsMixin(clientApplications)`](#fn-specinitproviderconditionswithclientapplicationsmixin)
      * [`fn withDevices(devices)`](#fn-specinitproviderconditionswithdevices)
      * [`fn withDevicesMixin(devices)`](#fn-specinitproviderconditionswithdevicesmixin)
      * [`fn withInsiderRiskLevels(insiderRiskLevels)`](#fn-specinitproviderconditionswithinsiderrisklevels)
      * [`fn withLocations(locations)`](#fn-specinitproviderconditionswithlocations)
      * [`fn withLocationsMixin(locations)`](#fn-specinitproviderconditionswithlocationsmixin)
      * [`fn withPlatforms(platforms)`](#fn-specinitproviderconditionswithplatforms)
      * [`fn withPlatformsMixin(platforms)`](#fn-specinitproviderconditionswithplatformsmixin)
      * [`fn withServicePrincipalRiskLevels(servicePrincipalRiskLevels)`](#fn-specinitproviderconditionswithserviceprincipalrisklevels)
      * [`fn withServicePrincipalRiskLevelsMixin(servicePrincipalRiskLevels)`](#fn-specinitproviderconditionswithserviceprincipalrisklevelsmixin)
      * [`fn withSignInRiskLevels(signInRiskLevels)`](#fn-specinitproviderconditionswithsigninrisklevels)
      * [`fn withSignInRiskLevelsMixin(signInRiskLevels)`](#fn-specinitproviderconditionswithsigninrisklevelsmixin)
      * [`fn withUserRiskLevels(userRiskLevels)`](#fn-specinitproviderconditionswithuserrisklevels)
      * [`fn withUserRiskLevelsMixin(userRiskLevels)`](#fn-specinitproviderconditionswithuserrisklevelsmixin)
      * [`fn withUsers(users)`](#fn-specinitproviderconditionswithusers)
      * [`fn withUsersMixin(users)`](#fn-specinitproviderconditionswithusersmixin)
      * [`obj spec.initProvider.conditions.applications`](#obj-specinitproviderconditionsapplications)
        * [`fn withExcludedApplications(excludedApplications)`](#fn-specinitproviderconditionsapplicationswithexcludedapplications)
        * [`fn withExcludedApplicationsMixin(excludedApplications)`](#fn-specinitproviderconditionsapplicationswithexcludedapplicationsmixin)
        * [`fn withIncludedApplications(includedApplications)`](#fn-specinitproviderconditionsapplicationswithincludedapplications)
        * [`fn withIncludedApplicationsMixin(includedApplications)`](#fn-specinitproviderconditionsapplicationswithincludedapplicationsmixin)
        * [`fn withIncludedUserActions(includedUserActions)`](#fn-specinitproviderconditionsapplicationswithincludeduseractions)
        * [`fn withIncludedUserActionsMixin(includedUserActions)`](#fn-specinitproviderconditionsapplicationswithincludeduseractionsmixin)
      * [`obj spec.initProvider.conditions.clientApplications`](#obj-specinitproviderconditionsclientapplications)
        * [`fn withExcludedServicePrincipals(excludedServicePrincipals)`](#fn-specinitproviderconditionsclientapplicationswithexcludedserviceprincipals)
        * [`fn withExcludedServicePrincipalsMixin(excludedServicePrincipals)`](#fn-specinitproviderconditionsclientapplicationswithexcludedserviceprincipalsmixin)
        * [`fn withIncludedServicePrincipals(includedServicePrincipals)`](#fn-specinitproviderconditionsclientapplicationswithincludedserviceprincipals)
        * [`fn withIncludedServicePrincipalsMixin(includedServicePrincipals)`](#fn-specinitproviderconditionsclientapplicationswithincludedserviceprincipalsmixin)
      * [`obj spec.initProvider.conditions.devices`](#obj-specinitproviderconditionsdevices)
        * [`fn withFilter(filter)`](#fn-specinitproviderconditionsdeviceswithfilter)
        * [`fn withFilterMixin(filter)`](#fn-specinitproviderconditionsdeviceswithfiltermixin)
        * [`obj spec.initProvider.conditions.devices.filter`](#obj-specinitproviderconditionsdevicesfilter)
          * [`fn withMode(mode)`](#fn-specinitproviderconditionsdevicesfilterwithmode)
          * [`fn withRule(rule)`](#fn-specinitproviderconditionsdevicesfilterwithrule)
      * [`obj spec.initProvider.conditions.locations`](#obj-specinitproviderconditionslocations)
        * [`fn withExcludedLocations(excludedLocations)`](#fn-specinitproviderconditionslocationswithexcludedlocations)
        * [`fn withExcludedLocationsMixin(excludedLocations)`](#fn-specinitproviderconditionslocationswithexcludedlocationsmixin)
        * [`fn withIncludedLocations(includedLocations)`](#fn-specinitproviderconditionslocationswithincludedlocations)
        * [`fn withIncludedLocationsMixin(includedLocations)`](#fn-specinitproviderconditionslocationswithincludedlocationsmixin)
      * [`obj spec.initProvider.conditions.platforms`](#obj-specinitproviderconditionsplatforms)
        * [`fn withExcludedPlatforms(excludedPlatforms)`](#fn-specinitproviderconditionsplatformswithexcludedplatforms)
        * [`fn withExcludedPlatformsMixin(excludedPlatforms)`](#fn-specinitproviderconditionsplatformswithexcludedplatformsmixin)
        * [`fn withIncludedPlatforms(includedPlatforms)`](#fn-specinitproviderconditionsplatformswithincludedplatforms)
        * [`fn withIncludedPlatformsMixin(includedPlatforms)`](#fn-specinitproviderconditionsplatformswithincludedplatformsmixin)
      * [`obj spec.initProvider.conditions.users`](#obj-specinitproviderconditionsusers)
        * [`fn withExcludedGroups(excludedGroups)`](#fn-specinitproviderconditionsuserswithexcludedgroups)
        * [`fn withExcludedGroupsMixin(excludedGroups)`](#fn-specinitproviderconditionsuserswithexcludedgroupsmixin)
        * [`fn withExcludedGuestsOrExternalUsers(excludedGuestsOrExternalUsers)`](#fn-specinitproviderconditionsuserswithexcludedguestsorexternalusers)
        * [`fn withExcludedGuestsOrExternalUsersMixin(excludedGuestsOrExternalUsers)`](#fn-specinitproviderconditionsuserswithexcludedguestsorexternalusersmixin)
        * [`fn withExcludedRoles(excludedRoles)`](#fn-specinitproviderconditionsuserswithexcludedroles)
        * [`fn withExcludedRolesMixin(excludedRoles)`](#fn-specinitproviderconditionsuserswithexcludedrolesmixin)
        * [`fn withExcludedUsers(excludedUsers)`](#fn-specinitproviderconditionsuserswithexcludedusers)
        * [`fn withExcludedUsersMixin(excludedUsers)`](#fn-specinitproviderconditionsuserswithexcludedusersmixin)
        * [`fn withIncludedGroups(includedGroups)`](#fn-specinitproviderconditionsuserswithincludedgroups)
        * [`fn withIncludedGroupsMixin(includedGroups)`](#fn-specinitproviderconditionsuserswithincludedgroupsmixin)
        * [`fn withIncludedGuestsOrExternalUsers(includedGuestsOrExternalUsers)`](#fn-specinitproviderconditionsuserswithincludedguestsorexternalusers)
        * [`fn withIncludedGuestsOrExternalUsersMixin(includedGuestsOrExternalUsers)`](#fn-specinitproviderconditionsuserswithincludedguestsorexternalusersmixin)
        * [`fn withIncludedRoles(includedRoles)`](#fn-specinitproviderconditionsuserswithincludedroles)
        * [`fn withIncludedRolesMixin(includedRoles)`](#fn-specinitproviderconditionsuserswithincludedrolesmixin)
        * [`fn withIncludedUsers(includedUsers)`](#fn-specinitproviderconditionsuserswithincludedusers)
        * [`fn withIncludedUsersMixin(includedUsers)`](#fn-specinitproviderconditionsuserswithincludedusersmixin)
        * [`obj spec.initProvider.conditions.users.excludedGuestsOrExternalUsers`](#obj-specinitproviderconditionsusersexcludedguestsorexternalusers)
          * [`fn withExternalTenants(externalTenants)`](#fn-specinitproviderconditionsusersexcludedguestsorexternaluserswithexternaltenants)
          * [`fn withExternalTenantsMixin(externalTenants)`](#fn-specinitproviderconditionsusersexcludedguestsorexternaluserswithexternaltenantsmixin)
          * [`fn withGuestOrExternalUserTypes(guestOrExternalUserTypes)`](#fn-specinitproviderconditionsusersexcludedguestsorexternaluserswithguestorexternalusertypes)
          * [`fn withGuestOrExternalUserTypesMixin(guestOrExternalUserTypes)`](#fn-specinitproviderconditionsusersexcludedguestsorexternaluserswithguestorexternalusertypesmixin)
          * [`obj spec.initProvider.conditions.users.excludedGuestsOrExternalUsers.externalTenants`](#obj-specinitproviderconditionsusersexcludedguestsorexternalusersexternaltenants)
            * [`fn withMembers(members)`](#fn-specinitproviderconditionsusersexcludedguestsorexternalusersexternaltenantswithmembers)
            * [`fn withMembersMixin(members)`](#fn-specinitproviderconditionsusersexcludedguestsorexternalusersexternaltenantswithmembersmixin)
            * [`fn withMembershipKind(membershipKind)`](#fn-specinitproviderconditionsusersexcludedguestsorexternalusersexternaltenantswithmembershipkind)
        * [`obj spec.initProvider.conditions.users.includedGuestsOrExternalUsers`](#obj-specinitproviderconditionsusersincludedguestsorexternalusers)
          * [`fn withExternalTenants(externalTenants)`](#fn-specinitproviderconditionsusersincludedguestsorexternaluserswithexternaltenants)
          * [`fn withExternalTenantsMixin(externalTenants)`](#fn-specinitproviderconditionsusersincludedguestsorexternaluserswithexternaltenantsmixin)
          * [`fn withGuestOrExternalUserTypes(guestOrExternalUserTypes)`](#fn-specinitproviderconditionsusersincludedguestsorexternaluserswithguestorexternalusertypes)
          * [`fn withGuestOrExternalUserTypesMixin(guestOrExternalUserTypes)`](#fn-specinitproviderconditionsusersincludedguestsorexternaluserswithguestorexternalusertypesmixin)
          * [`obj spec.initProvider.conditions.users.includedGuestsOrExternalUsers.externalTenants`](#obj-specinitproviderconditionsusersincludedguestsorexternalusersexternaltenants)
            * [`fn withMembers(members)`](#fn-specinitproviderconditionsusersincludedguestsorexternalusersexternaltenantswithmembers)
            * [`fn withMembersMixin(members)`](#fn-specinitproviderconditionsusersincludedguestsorexternalusersexternaltenantswithmembersmixin)
            * [`fn withMembershipKind(membershipKind)`](#fn-specinitproviderconditionsusersincludedguestsorexternalusersexternaltenantswithmembershipkind)
    * [`obj spec.initProvider.grantControls`](#obj-specinitprovidergrantcontrols)
      * [`fn withAuthenticationStrengthPolicyId(authenticationStrengthPolicyId)`](#fn-specinitprovidergrantcontrolswithauthenticationstrengthpolicyid)
      * [`fn withBuiltInControls(builtInControls)`](#fn-specinitprovidergrantcontrolswithbuiltincontrols)
      * [`fn withBuiltInControlsMixin(builtInControls)`](#fn-specinitprovidergrantcontrolswithbuiltincontrolsmixin)
      * [`fn withCustomAuthenticationFactors(customAuthenticationFactors)`](#fn-specinitprovidergrantcontrolswithcustomauthenticationfactors)
      * [`fn withCustomAuthenticationFactorsMixin(customAuthenticationFactors)`](#fn-specinitprovidergrantcontrolswithcustomauthenticationfactorsmixin)
      * [`fn withOperator(operator)`](#fn-specinitprovidergrantcontrolswithoperator)
      * [`fn withTermsOfUse(termsOfUse)`](#fn-specinitprovidergrantcontrolswithtermsofuse)
      * [`fn withTermsOfUseMixin(termsOfUse)`](#fn-specinitprovidergrantcontrolswithtermsofusemixin)
    * [`obj spec.initProvider.sessionControls`](#obj-specinitprovidersessioncontrols)
      * [`fn withApplicationEnforcedRestrictionsEnabled(applicationEnforcedRestrictionsEnabled)`](#fn-specinitprovidersessioncontrolswithapplicationenforcedrestrictionsenabled)
      * [`fn withCloudAppSecurityPolicy(cloudAppSecurityPolicy)`](#fn-specinitprovidersessioncontrolswithcloudappsecuritypolicy)
      * [`fn withDisableResilienceDefaults(disableResilienceDefaults)`](#fn-specinitprovidersessioncontrolswithdisableresiliencedefaults)
      * [`fn withPersistentBrowserMode(persistentBrowserMode)`](#fn-specinitprovidersessioncontrolswithpersistentbrowsermode)
      * [`fn withSignInFrequency(signInFrequency)`](#fn-specinitprovidersessioncontrolswithsigninfrequency)
      * [`fn withSignInFrequencyAuthenticationType(signInFrequencyAuthenticationType)`](#fn-specinitprovidersessioncontrolswithsigninfrequencyauthenticationtype)
      * [`fn withSignInFrequencyInterval(signInFrequencyInterval)`](#fn-specinitprovidersessioncontrolswithsigninfrequencyinterval)
      * [`fn withSignInFrequencyPeriod(signInFrequencyPeriod)`](#fn-specinitprovidersessioncontrolswithsigninfrequencyperiod)
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

new returns an instance of AccessPolicy

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

"AccessPolicySpec defines the desired state of AccessPolicy"

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



### fn spec.forProvider.withConditions

```ts
withConditions(conditions)
```

"A conditions block as documented below, which specifies the rules that must be met for the policy to apply."

### fn spec.forProvider.withConditionsMixin

```ts
withConditionsMixin(conditions)
```

"A conditions block as documented below, which specifies the rules that must be met for the policy to apply."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withDisplayName

```ts
withDisplayName(displayName)
```

"The friendly name for this Conditional Access Policy."

### fn spec.forProvider.withGrantControls

```ts
withGrantControls(grantControls)
```

"A grant_controls block as documented below, which specifies the grant controls that must be fulfilled to pass the policy."

### fn spec.forProvider.withGrantControlsMixin

```ts
withGrantControlsMixin(grantControls)
```

"A grant_controls block as documented below, which specifies the grant controls that must be fulfilled to pass the policy."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withSessionControls

```ts
withSessionControls(sessionControls)
```

"A session_controls block as documented below, which specifies the session controls that are enforced after sign-in."

### fn spec.forProvider.withSessionControlsMixin

```ts
withSessionControlsMixin(sessionControls)
```

"A session_controls block as documented below, which specifies the session controls that are enforced after sign-in."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.withState

```ts
withState(state)
```

"Specifies the state of the policy object. Possible values are: enabled, disabled and enabledForReportingButNotEnforced"

## obj spec.forProvider.conditions

"A conditions block as documented below, which specifies the rules that must be met for the policy to apply."

### fn spec.forProvider.conditions.withApplications

```ts
withApplications(applications)
```

"An applications block as documented below, which specifies applications and user actions included in and excluded from the policy."

### fn spec.forProvider.conditions.withApplicationsMixin

```ts
withApplicationsMixin(applications)
```

"An applications block as documented below, which specifies applications and user actions included in and excluded from the policy."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.withClientAppTypes

```ts
withClientAppTypes(clientAppTypes)
```

"A list of client application types included in the policy. Possible values are: all, browser, mobileAppsAndDesktopClients, exchangeActiveSync, easSupported and other."

### fn spec.forProvider.conditions.withClientAppTypesMixin

```ts
withClientAppTypesMixin(clientAppTypes)
```

"A list of client application types included in the policy. Possible values are: all, browser, mobileAppsAndDesktopClients, exchangeActiveSync, easSupported and other."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.withClientApplications

```ts
withClientApplications(clientApplications)
```

"An client_applications block as documented below, which specifies service principals included in and excluded from the policy."

### fn spec.forProvider.conditions.withClientApplicationsMixin

```ts
withClientApplicationsMixin(clientApplications)
```

"An client_applications block as documented below, which specifies service principals included in and excluded from the policy."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.withDevices

```ts
withDevices(devices)
```

"A devices block as documented below, which describes devices to be included in and excluded from the policy. A devices block can be added to an existing policy, but removing the devices block forces a new resource to be created."

### fn spec.forProvider.conditions.withDevicesMixin

```ts
withDevicesMixin(devices)
```

"A devices block as documented below, which describes devices to be included in and excluded from the policy. A devices block can be added to an existing policy, but removing the devices block forces a new resource to be created."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.withInsiderRiskLevels

```ts
withInsiderRiskLevels(insiderRiskLevels)
```

"The insider risk level in the policy. Possible values are: minor, moderate, elevated, unknownFutureValue."

### fn spec.forProvider.conditions.withLocations

```ts
withLocations(locations)
```

"A locations block as documented below, which specifies locations included in and excluded from the policy."

### fn spec.forProvider.conditions.withLocationsMixin

```ts
withLocationsMixin(locations)
```

"A locations block as documented below, which specifies locations included in and excluded from the policy."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.withPlatforms

```ts
withPlatforms(platforms)
```

"A platforms block as documented below, which specifies platforms included in and excluded from the policy."

### fn spec.forProvider.conditions.withPlatformsMixin

```ts
withPlatformsMixin(platforms)
```

"A platforms block as documented below, which specifies platforms included in and excluded from the policy."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.withServicePrincipalRiskLevels

```ts
withServicePrincipalRiskLevels(servicePrincipalRiskLevels)
```

"A list of service principal sign-in risk levels included in the policy. Possible values are: low, medium, high, none, unknownFutureValue."

### fn spec.forProvider.conditions.withServicePrincipalRiskLevelsMixin

```ts
withServicePrincipalRiskLevelsMixin(servicePrincipalRiskLevels)
```

"A list of service principal sign-in risk levels included in the policy. Possible values are: low, medium, high, none, unknownFutureValue."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.withSignInRiskLevels

```ts
withSignInRiskLevels(signInRiskLevels)
```

"A list of user sign-in risk levels included in the policy. Possible values are: low, medium, high, hidden, none, unknownFutureValue."

### fn spec.forProvider.conditions.withSignInRiskLevelsMixin

```ts
withSignInRiskLevelsMixin(signInRiskLevels)
```

"A list of user sign-in risk levels included in the policy. Possible values are: low, medium, high, hidden, none, unknownFutureValue."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.withUserRiskLevels

```ts
withUserRiskLevels(userRiskLevels)
```

"A list of user risk levels included in the policy. Possible values are: low, medium, high, hidden, none, unknownFutureValue."

### fn spec.forProvider.conditions.withUserRiskLevelsMixin

```ts
withUserRiskLevelsMixin(userRiskLevels)
```

"A list of user risk levels included in the policy. Possible values are: low, medium, high, hidden, none, unknownFutureValue."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.withUsers

```ts
withUsers(users)
```

"A users block as documented below, which specifies users, groups, and roles included in and excluded from the policy."

### fn spec.forProvider.conditions.withUsersMixin

```ts
withUsersMixin(users)
```

"A users block as documented below, which specifies users, groups, and roles included in and excluded from the policy."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.conditions.applications

"An applications block as documented below, which specifies applications and user actions included in and excluded from the policy."

### fn spec.forProvider.conditions.applications.withExcludedApplications

```ts
withExcludedApplications(excludedApplications)
```

"A list of application IDs explicitly excluded from the policy. Can also be set to Office365."

### fn spec.forProvider.conditions.applications.withExcludedApplicationsMixin

```ts
withExcludedApplicationsMixin(excludedApplications)
```

"A list of application IDs explicitly excluded from the policy. Can also be set to Office365."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.applications.withIncludedApplications

```ts
withIncludedApplications(includedApplications)
```

"A list of application IDs the policy applies to, unless explicitly excluded (in excluded_applications). Can also be set to All, None or Office365. Cannot be specified with included_user_actions. One of included_applications or included_user_actions must be specified."

### fn spec.forProvider.conditions.applications.withIncludedApplicationsMixin

```ts
withIncludedApplicationsMixin(includedApplications)
```

"A list of application IDs the policy applies to, unless explicitly excluded (in excluded_applications). Can also be set to All, None or Office365. Cannot be specified with included_user_actions. One of included_applications or included_user_actions must be specified."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.applications.withIncludedUserActions

```ts
withIncludedUserActions(includedUserActions)
```

"A list of user actions to include. Supported values are urn:user:registerdevice and urn:user:registersecurityinfo. Cannot be specified with included_applications. One of included_applications or included_user_actions must be specified."

### fn spec.forProvider.conditions.applications.withIncludedUserActionsMixin

```ts
withIncludedUserActionsMixin(includedUserActions)
```

"A list of user actions to include. Supported values are urn:user:registerdevice and urn:user:registersecurityinfo. Cannot be specified with included_applications. One of included_applications or included_user_actions must be specified."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.conditions.clientApplications

"An client_applications block as documented below, which specifies service principals included in and excluded from the policy."

### fn spec.forProvider.conditions.clientApplications.withExcludedServicePrincipals

```ts
withExcludedServicePrincipals(excludedServicePrincipals)
```

"A list of service principal IDs explicitly excluded in the policy."

### fn spec.forProvider.conditions.clientApplications.withExcludedServicePrincipalsMixin

```ts
withExcludedServicePrincipalsMixin(excludedServicePrincipals)
```

"A list of service principal IDs explicitly excluded in the policy."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.clientApplications.withIncludedServicePrincipals

```ts
withIncludedServicePrincipals(includedServicePrincipals)
```

"A list of service principal IDs explicitly included in the policy. Can be set to ServicePrincipalsInMyTenant to include all service principals. This is mandatory value when at least one excluded_service_principals is set."

### fn spec.forProvider.conditions.clientApplications.withIncludedServicePrincipalsMixin

```ts
withIncludedServicePrincipalsMixin(includedServicePrincipals)
```

"A list of service principal IDs explicitly included in the policy. Can be set to ServicePrincipalsInMyTenant to include all service principals. This is mandatory value when at least one excluded_service_principals is set."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.conditions.devices

"A devices block as documented below, which describes devices to be included in and excluded from the policy. A devices block can be added to an existing policy, but removing the devices block forces a new resource to be created."

### fn spec.forProvider.conditions.devices.withFilter

```ts
withFilter(filter)
```

"A filter block as described below."

### fn spec.forProvider.conditions.devices.withFilterMixin

```ts
withFilterMixin(filter)
```

"A filter block as described below."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.conditions.devices.filter

"A filter block as described below."

### fn spec.forProvider.conditions.devices.filter.withMode

```ts
withMode(mode)
```

"Whether to include in, or exclude from, matching devices from the policy. Supported values are include or exclude."

### fn spec.forProvider.conditions.devices.filter.withRule

```ts
withRule(rule)
```

"Condition filter to match devices. For more information, see official documentation."

## obj spec.forProvider.conditions.locations

"A locations block as documented below, which specifies locations included in and excluded from the policy."

### fn spec.forProvider.conditions.locations.withExcludedLocations

```ts
withExcludedLocations(excludedLocations)
```

"A list of location IDs excluded from scope of policy. Can also be set to AllTrusted."

### fn spec.forProvider.conditions.locations.withExcludedLocationsMixin

```ts
withExcludedLocationsMixin(excludedLocations)
```

"A list of location IDs excluded from scope of policy. Can also be set to AllTrusted."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.locations.withIncludedLocations

```ts
withIncludedLocations(includedLocations)
```

"A list of location IDs in scope of policy unless explicitly excluded. Can also be set to All, or AllTrusted."

### fn spec.forProvider.conditions.locations.withIncludedLocationsMixin

```ts
withIncludedLocationsMixin(includedLocations)
```

"A list of location IDs in scope of policy unless explicitly excluded. Can also be set to All, or AllTrusted."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.conditions.platforms

"A platforms block as documented below, which specifies platforms included in and excluded from the policy."

### fn spec.forProvider.conditions.platforms.withExcludedPlatforms

```ts
withExcludedPlatforms(excludedPlatforms)
```

"A list of platforms explicitly excluded from the policy. Possible values are: all, android, iOS, linux, macOS, windows, windowsPhone or unknownFutureValue."

### fn spec.forProvider.conditions.platforms.withExcludedPlatformsMixin

```ts
withExcludedPlatformsMixin(excludedPlatforms)
```

"A list of platforms explicitly excluded from the policy. Possible values are: all, android, iOS, linux, macOS, windows, windowsPhone or unknownFutureValue."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.platforms.withIncludedPlatforms

```ts
withIncludedPlatforms(includedPlatforms)
```

"A list of platforms the policy applies to, unless explicitly excluded. Possible values are: all, android, iOS, linux, macOS, windows, windowsPhone or unknownFutureValue."

### fn spec.forProvider.conditions.platforms.withIncludedPlatformsMixin

```ts
withIncludedPlatformsMixin(includedPlatforms)
```

"A list of platforms the policy applies to, unless explicitly excluded. Possible values are: all, android, iOS, linux, macOS, windows, windowsPhone or unknownFutureValue."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.conditions.users

"A users block as documented below, which specifies users, groups, and roles included in and excluded from the policy."

### fn spec.forProvider.conditions.users.withExcludedGroups

```ts
withExcludedGroups(excludedGroups)
```

"A list of group IDs excluded from scope of policy."

### fn spec.forProvider.conditions.users.withExcludedGroupsMixin

```ts
withExcludedGroupsMixin(excludedGroups)
```

"A list of group IDs excluded from scope of policy."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.users.withExcludedGuestsOrExternalUsers

```ts
withExcludedGuestsOrExternalUsers(excludedGuestsOrExternalUsers)
```

"A guests_or_external_users block as documented below, which specifies internal guests and external users excluded from scope of policy."

### fn spec.forProvider.conditions.users.withExcludedGuestsOrExternalUsersMixin

```ts
withExcludedGuestsOrExternalUsersMixin(excludedGuestsOrExternalUsers)
```

"A guests_or_external_users block as documented below, which specifies internal guests and external users excluded from scope of policy."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.users.withExcludedRoles

```ts
withExcludedRoles(excludedRoles)
```

"A list of role IDs excluded from scope of policy."

### fn spec.forProvider.conditions.users.withExcludedRolesMixin

```ts
withExcludedRolesMixin(excludedRoles)
```

"A list of role IDs excluded from scope of policy."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.users.withExcludedUsers

```ts
withExcludedUsers(excludedUsers)
```

"A list of user IDs excluded from scope of policy and/or GuestsOrExternalUsers."

### fn spec.forProvider.conditions.users.withExcludedUsersMixin

```ts
withExcludedUsersMixin(excludedUsers)
```

"A list of user IDs excluded from scope of policy and/or GuestsOrExternalUsers."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.users.withIncludedGroups

```ts
withIncludedGroups(includedGroups)
```

"A list of group IDs in scope of policy unless explicitly excluded."

### fn spec.forProvider.conditions.users.withIncludedGroupsMixin

```ts
withIncludedGroupsMixin(includedGroups)
```

"A list of group IDs in scope of policy unless explicitly excluded."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.users.withIncludedGuestsOrExternalUsers

```ts
withIncludedGuestsOrExternalUsers(includedGuestsOrExternalUsers)
```

"A guests_or_external_users block as documented below, which specifies internal guests and external users in scope of policy."

### fn spec.forProvider.conditions.users.withIncludedGuestsOrExternalUsersMixin

```ts
withIncludedGuestsOrExternalUsersMixin(includedGuestsOrExternalUsers)
```

"A guests_or_external_users block as documented below, which specifies internal guests and external users in scope of policy."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.users.withIncludedRoles

```ts
withIncludedRoles(includedRoles)
```

"A list of role IDs in scope of policy unless explicitly excluded."

### fn spec.forProvider.conditions.users.withIncludedRolesMixin

```ts
withIncludedRolesMixin(includedRoles)
```

"A list of role IDs in scope of policy unless explicitly excluded."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.users.withIncludedUsers

```ts
withIncludedUsers(includedUsers)
```

"A list of user IDs in scope of policy unless explicitly excluded, or None or All or GuestsOrExternalUsers."

### fn spec.forProvider.conditions.users.withIncludedUsersMixin

```ts
withIncludedUsersMixin(includedUsers)
```

"A list of user IDs in scope of policy unless explicitly excluded, or None or All or GuestsOrExternalUsers."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.conditions.users.excludedGuestsOrExternalUsers

"A guests_or_external_users block as documented below, which specifies internal guests and external users excluded from scope of policy."

### fn spec.forProvider.conditions.users.excludedGuestsOrExternalUsers.withExternalTenants

```ts
withExternalTenants(externalTenants)
```

"An external_tenants block as documented below, which specifies external tenants in a policy scope."

### fn spec.forProvider.conditions.users.excludedGuestsOrExternalUsers.withExternalTenantsMixin

```ts
withExternalTenantsMixin(externalTenants)
```

"An external_tenants block as documented below, which specifies external tenants in a policy scope."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.users.excludedGuestsOrExternalUsers.withGuestOrExternalUserTypes

```ts
withGuestOrExternalUserTypes(guestOrExternalUserTypes)
```

"A list of guest or external user types. Possible values are: b2bCollaborationGuest, b2bCollaborationMember, b2bDirectConnectUser, internalGuest, none, otherExternalUser, serviceProvider, unknownFutureValue."

### fn spec.forProvider.conditions.users.excludedGuestsOrExternalUsers.withGuestOrExternalUserTypesMixin

```ts
withGuestOrExternalUserTypesMixin(guestOrExternalUserTypes)
```

"A list of guest or external user types. Possible values are: b2bCollaborationGuest, b2bCollaborationMember, b2bDirectConnectUser, internalGuest, none, otherExternalUser, serviceProvider, unknownFutureValue."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.conditions.users.excludedGuestsOrExternalUsers.externalTenants

"An external_tenants block as documented below, which specifies external tenants in a policy scope."

### fn spec.forProvider.conditions.users.excludedGuestsOrExternalUsers.externalTenants.withMembers

```ts
withMembers(members)
```

"A list tenant IDs. Can only be specified if membership_kind is enumerated."

### fn spec.forProvider.conditions.users.excludedGuestsOrExternalUsers.externalTenants.withMembersMixin

```ts
withMembersMixin(members)
```

"A list tenant IDs. Can only be specified if membership_kind is enumerated."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.users.excludedGuestsOrExternalUsers.externalTenants.withMembershipKind

```ts
withMembershipKind(membershipKind)
```

"The external tenant membership kind. Possible values are: all, enumerated, unknownFutureValue."

## obj spec.forProvider.conditions.users.includedGuestsOrExternalUsers

"A guests_or_external_users block as documented below, which specifies internal guests and external users in scope of policy."

### fn spec.forProvider.conditions.users.includedGuestsOrExternalUsers.withExternalTenants

```ts
withExternalTenants(externalTenants)
```

"An external_tenants block as documented below, which specifies external tenants in a policy scope."

### fn spec.forProvider.conditions.users.includedGuestsOrExternalUsers.withExternalTenantsMixin

```ts
withExternalTenantsMixin(externalTenants)
```

"An external_tenants block as documented below, which specifies external tenants in a policy scope."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.users.includedGuestsOrExternalUsers.withGuestOrExternalUserTypes

```ts
withGuestOrExternalUserTypes(guestOrExternalUserTypes)
```

"A list of guest or external user types. Possible values are: b2bCollaborationGuest, b2bCollaborationMember, b2bDirectConnectUser, internalGuest, none, otherExternalUser, serviceProvider, unknownFutureValue."

### fn spec.forProvider.conditions.users.includedGuestsOrExternalUsers.withGuestOrExternalUserTypesMixin

```ts
withGuestOrExternalUserTypesMixin(guestOrExternalUserTypes)
```

"A list of guest or external user types. Possible values are: b2bCollaborationGuest, b2bCollaborationMember, b2bDirectConnectUser, internalGuest, none, otherExternalUser, serviceProvider, unknownFutureValue."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.conditions.users.includedGuestsOrExternalUsers.externalTenants

"An external_tenants block as documented below, which specifies external tenants in a policy scope."

### fn spec.forProvider.conditions.users.includedGuestsOrExternalUsers.externalTenants.withMembers

```ts
withMembers(members)
```

"A list tenant IDs. Can only be specified if membership_kind is enumerated."

### fn spec.forProvider.conditions.users.includedGuestsOrExternalUsers.externalTenants.withMembersMixin

```ts
withMembersMixin(members)
```

"A list tenant IDs. Can only be specified if membership_kind is enumerated."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.conditions.users.includedGuestsOrExternalUsers.externalTenants.withMembershipKind

```ts
withMembershipKind(membershipKind)
```

"The external tenant membership kind. Possible values are: all, enumerated, unknownFutureValue."

## obj spec.forProvider.grantControls

"A grant_controls block as documented below, which specifies the grant controls that must be fulfilled to pass the policy."

### fn spec.forProvider.grantControls.withAuthenticationStrengthPolicyId

```ts
withAuthenticationStrengthPolicyId(authenticationStrengthPolicyId)
```

"ID of an Authentication Strength Policy to use in this policy. When using a hard-coded ID, the UUID value should be prefixed with: /policies/authenticationStrengthPolicies/."

### fn spec.forProvider.grantControls.withBuiltInControls

```ts
withBuiltInControls(builtInControls)
```

"List of built-in controls required by the policy. Possible values are: block, mfa, approvedApplication, compliantApplication, compliantDevice, domainJoinedDevice, passwordChange or unknownFutureValue."

### fn spec.forProvider.grantControls.withBuiltInControlsMixin

```ts
withBuiltInControlsMixin(builtInControls)
```

"List of built-in controls required by the policy. Possible values are: block, mfa, approvedApplication, compliantApplication, compliantDevice, domainJoinedDevice, passwordChange or unknownFutureValue."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.grantControls.withCustomAuthenticationFactors

```ts
withCustomAuthenticationFactors(customAuthenticationFactors)
```

"List of custom controls IDs required by the policy."

### fn spec.forProvider.grantControls.withCustomAuthenticationFactorsMixin

```ts
withCustomAuthenticationFactorsMixin(customAuthenticationFactors)
```

"List of custom controls IDs required by the policy."

**Note:** This function appends passed data to existing values

### fn spec.forProvider.grantControls.withOperator

```ts
withOperator(operator)
```

"Defines the relationship of the grant controls. Possible values are: AND, OR."

### fn spec.forProvider.grantControls.withTermsOfUse

```ts
withTermsOfUse(termsOfUse)
```

"List of terms of use IDs required by the policy."

### fn spec.forProvider.grantControls.withTermsOfUseMixin

```ts
withTermsOfUseMixin(termsOfUse)
```

"List of terms of use IDs required by the policy."

**Note:** This function appends passed data to existing values

## obj spec.forProvider.sessionControls

"A session_controls block as documented below, which specifies the session controls that are enforced after sign-in."

### fn spec.forProvider.sessionControls.withApplicationEnforcedRestrictionsEnabled

```ts
withApplicationEnforcedRestrictionsEnabled(applicationEnforcedRestrictionsEnabled)
```

"Whether application enforced restrictions are enabled. Defaults to false."

### fn spec.forProvider.sessionControls.withCloudAppSecurityPolicy

```ts
withCloudAppSecurityPolicy(cloudAppSecurityPolicy)
```

"Enables cloud app security and specifies the cloud app security policy to use. Possible values are: blockDownloads, mcasConfigured, monitorOnly or unknownFutureValue."

### fn spec.forProvider.sessionControls.withDisableResilienceDefaults

```ts
withDisableResilienceDefaults(disableResilienceDefaults)
```

"Disables resilience defaults. Defaults to false."

### fn spec.forProvider.sessionControls.withPersistentBrowserMode

```ts
withPersistentBrowserMode(persistentBrowserMode)
```

"Session control to define whether to persist cookies. Possible values are: always or never."

### fn spec.forProvider.sessionControls.withSignInFrequency

```ts
withSignInFrequency(signInFrequency)
```

"Number of days or hours to enforce sign-in frequency. Required when sign_in_frequency_period is specified."

### fn spec.forProvider.sessionControls.withSignInFrequencyAuthenticationType

```ts
withSignInFrequencyAuthenticationType(signInFrequencyAuthenticationType)
```

"Authentication type for enforcing sign-in frequency. Possible values are: primaryAndSecondaryAuthentication or secondaryAuthentication. Defaults to primaryAndSecondaryAuthentication."

### fn spec.forProvider.sessionControls.withSignInFrequencyInterval

```ts
withSignInFrequencyInterval(signInFrequencyInterval)
```

"The interval to apply to sign-in frequency control. Possible values are: timeBased or everyTime. Defaults to timeBased."

### fn spec.forProvider.sessionControls.withSignInFrequencyPeriod

```ts
withSignInFrequencyPeriod(signInFrequencyPeriod)
```

"The time period to enforce sign-in frequency. Possible values are: hours or days. Required when sign_in_frequency_period is specified."

## obj spec.initProvider

"THIS IS A BETA FIELD. It will be honored\nunless the Management Policies feature flag is disabled.\nInitProvider holds the same fields as ForProvider, with the exception\nof Identifier and other resource reference fields. The fields that are\nin InitProvider are merged into ForProvider when the resource is created.\nThe same fields are also added to the terraform ignore_changes hook, to\navoid updating them after creation. This is useful for fields that are\nrequired on creation, but we do not desire to update them after creation,\nfor example because of an external controller is managing them, like an\nautoscaler."

### fn spec.initProvider.withConditions

```ts
withConditions(conditions)
```

"A conditions block as documented below, which specifies the rules that must be met for the policy to apply."

### fn spec.initProvider.withConditionsMixin

```ts
withConditionsMixin(conditions)
```

"A conditions block as documented below, which specifies the rules that must be met for the policy to apply."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withDisplayName

```ts
withDisplayName(displayName)
```

"The friendly name for this Conditional Access Policy."

### fn spec.initProvider.withGrantControls

```ts
withGrantControls(grantControls)
```

"A grant_controls block as documented below, which specifies the grant controls that must be fulfilled to pass the policy."

### fn spec.initProvider.withGrantControlsMixin

```ts
withGrantControlsMixin(grantControls)
```

"A grant_controls block as documented below, which specifies the grant controls that must be fulfilled to pass the policy."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withSessionControls

```ts
withSessionControls(sessionControls)
```

"A session_controls block as documented below, which specifies the session controls that are enforced after sign-in."

### fn spec.initProvider.withSessionControlsMixin

```ts
withSessionControlsMixin(sessionControls)
```

"A session_controls block as documented below, which specifies the session controls that are enforced after sign-in."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.withState

```ts
withState(state)
```

"Specifies the state of the policy object. Possible values are: enabled, disabled and enabledForReportingButNotEnforced"

## obj spec.initProvider.conditions

"A conditions block as documented below, which specifies the rules that must be met for the policy to apply."

### fn spec.initProvider.conditions.withApplications

```ts
withApplications(applications)
```

"An applications block as documented below, which specifies applications and user actions included in and excluded from the policy."

### fn spec.initProvider.conditions.withApplicationsMixin

```ts
withApplicationsMixin(applications)
```

"An applications block as documented below, which specifies applications and user actions included in and excluded from the policy."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.withClientAppTypes

```ts
withClientAppTypes(clientAppTypes)
```

"A list of client application types included in the policy. Possible values are: all, browser, mobileAppsAndDesktopClients, exchangeActiveSync, easSupported and other."

### fn spec.initProvider.conditions.withClientAppTypesMixin

```ts
withClientAppTypesMixin(clientAppTypes)
```

"A list of client application types included in the policy. Possible values are: all, browser, mobileAppsAndDesktopClients, exchangeActiveSync, easSupported and other."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.withClientApplications

```ts
withClientApplications(clientApplications)
```

"An client_applications block as documented below, which specifies service principals included in and excluded from the policy."

### fn spec.initProvider.conditions.withClientApplicationsMixin

```ts
withClientApplicationsMixin(clientApplications)
```

"An client_applications block as documented below, which specifies service principals included in and excluded from the policy."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.withDevices

```ts
withDevices(devices)
```

"A devices block as documented below, which describes devices to be included in and excluded from the policy. A devices block can be added to an existing policy, but removing the devices block forces a new resource to be created."

### fn spec.initProvider.conditions.withDevicesMixin

```ts
withDevicesMixin(devices)
```

"A devices block as documented below, which describes devices to be included in and excluded from the policy. A devices block can be added to an existing policy, but removing the devices block forces a new resource to be created."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.withInsiderRiskLevels

```ts
withInsiderRiskLevels(insiderRiskLevels)
```

"The insider risk level in the policy. Possible values are: minor, moderate, elevated, unknownFutureValue."

### fn spec.initProvider.conditions.withLocations

```ts
withLocations(locations)
```

"A locations block as documented below, which specifies locations included in and excluded from the policy."

### fn spec.initProvider.conditions.withLocationsMixin

```ts
withLocationsMixin(locations)
```

"A locations block as documented below, which specifies locations included in and excluded from the policy."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.withPlatforms

```ts
withPlatforms(platforms)
```

"A platforms block as documented below, which specifies platforms included in and excluded from the policy."

### fn spec.initProvider.conditions.withPlatformsMixin

```ts
withPlatformsMixin(platforms)
```

"A platforms block as documented below, which specifies platforms included in and excluded from the policy."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.withServicePrincipalRiskLevels

```ts
withServicePrincipalRiskLevels(servicePrincipalRiskLevels)
```

"A list of service principal sign-in risk levels included in the policy. Possible values are: low, medium, high, none, unknownFutureValue."

### fn spec.initProvider.conditions.withServicePrincipalRiskLevelsMixin

```ts
withServicePrincipalRiskLevelsMixin(servicePrincipalRiskLevels)
```

"A list of service principal sign-in risk levels included in the policy. Possible values are: low, medium, high, none, unknownFutureValue."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.withSignInRiskLevels

```ts
withSignInRiskLevels(signInRiskLevels)
```

"A list of user sign-in risk levels included in the policy. Possible values are: low, medium, high, hidden, none, unknownFutureValue."

### fn spec.initProvider.conditions.withSignInRiskLevelsMixin

```ts
withSignInRiskLevelsMixin(signInRiskLevels)
```

"A list of user sign-in risk levels included in the policy. Possible values are: low, medium, high, hidden, none, unknownFutureValue."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.withUserRiskLevels

```ts
withUserRiskLevels(userRiskLevels)
```

"A list of user risk levels included in the policy. Possible values are: low, medium, high, hidden, none, unknownFutureValue."

### fn spec.initProvider.conditions.withUserRiskLevelsMixin

```ts
withUserRiskLevelsMixin(userRiskLevels)
```

"A list of user risk levels included in the policy. Possible values are: low, medium, high, hidden, none, unknownFutureValue."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.withUsers

```ts
withUsers(users)
```

"A users block as documented below, which specifies users, groups, and roles included in and excluded from the policy."

### fn spec.initProvider.conditions.withUsersMixin

```ts
withUsersMixin(users)
```

"A users block as documented below, which specifies users, groups, and roles included in and excluded from the policy."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.conditions.applications

"An applications block as documented below, which specifies applications and user actions included in and excluded from the policy."

### fn spec.initProvider.conditions.applications.withExcludedApplications

```ts
withExcludedApplications(excludedApplications)
```

"A list of application IDs explicitly excluded from the policy. Can also be set to Office365."

### fn spec.initProvider.conditions.applications.withExcludedApplicationsMixin

```ts
withExcludedApplicationsMixin(excludedApplications)
```

"A list of application IDs explicitly excluded from the policy. Can also be set to Office365."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.applications.withIncludedApplications

```ts
withIncludedApplications(includedApplications)
```

"A list of application IDs the policy applies to, unless explicitly excluded (in excluded_applications). Can also be set to All, None or Office365. Cannot be specified with included_user_actions. One of included_applications or included_user_actions must be specified."

### fn spec.initProvider.conditions.applications.withIncludedApplicationsMixin

```ts
withIncludedApplicationsMixin(includedApplications)
```

"A list of application IDs the policy applies to, unless explicitly excluded (in excluded_applications). Can also be set to All, None or Office365. Cannot be specified with included_user_actions. One of included_applications or included_user_actions must be specified."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.applications.withIncludedUserActions

```ts
withIncludedUserActions(includedUserActions)
```

"A list of user actions to include. Supported values are urn:user:registerdevice and urn:user:registersecurityinfo. Cannot be specified with included_applications. One of included_applications or included_user_actions must be specified."

### fn spec.initProvider.conditions.applications.withIncludedUserActionsMixin

```ts
withIncludedUserActionsMixin(includedUserActions)
```

"A list of user actions to include. Supported values are urn:user:registerdevice and urn:user:registersecurityinfo. Cannot be specified with included_applications. One of included_applications or included_user_actions must be specified."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.conditions.clientApplications

"An client_applications block as documented below, which specifies service principals included in and excluded from the policy."

### fn spec.initProvider.conditions.clientApplications.withExcludedServicePrincipals

```ts
withExcludedServicePrincipals(excludedServicePrincipals)
```

"A list of service principal IDs explicitly excluded in the policy."

### fn spec.initProvider.conditions.clientApplications.withExcludedServicePrincipalsMixin

```ts
withExcludedServicePrincipalsMixin(excludedServicePrincipals)
```

"A list of service principal IDs explicitly excluded in the policy."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.clientApplications.withIncludedServicePrincipals

```ts
withIncludedServicePrincipals(includedServicePrincipals)
```

"A list of service principal IDs explicitly included in the policy. Can be set to ServicePrincipalsInMyTenant to include all service principals. This is mandatory value when at least one excluded_service_principals is set."

### fn spec.initProvider.conditions.clientApplications.withIncludedServicePrincipalsMixin

```ts
withIncludedServicePrincipalsMixin(includedServicePrincipals)
```

"A list of service principal IDs explicitly included in the policy. Can be set to ServicePrincipalsInMyTenant to include all service principals. This is mandatory value when at least one excluded_service_principals is set."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.conditions.devices

"A devices block as documented below, which describes devices to be included in and excluded from the policy. A devices block can be added to an existing policy, but removing the devices block forces a new resource to be created."

### fn spec.initProvider.conditions.devices.withFilter

```ts
withFilter(filter)
```

"A filter block as described below."

### fn spec.initProvider.conditions.devices.withFilterMixin

```ts
withFilterMixin(filter)
```

"A filter block as described below."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.conditions.devices.filter

"A filter block as described below."

### fn spec.initProvider.conditions.devices.filter.withMode

```ts
withMode(mode)
```

"Whether to include in, or exclude from, matching devices from the policy. Supported values are include or exclude."

### fn spec.initProvider.conditions.devices.filter.withRule

```ts
withRule(rule)
```

"Condition filter to match devices. For more information, see official documentation."

## obj spec.initProvider.conditions.locations

"A locations block as documented below, which specifies locations included in and excluded from the policy."

### fn spec.initProvider.conditions.locations.withExcludedLocations

```ts
withExcludedLocations(excludedLocations)
```

"A list of location IDs excluded from scope of policy. Can also be set to AllTrusted."

### fn spec.initProvider.conditions.locations.withExcludedLocationsMixin

```ts
withExcludedLocationsMixin(excludedLocations)
```

"A list of location IDs excluded from scope of policy. Can also be set to AllTrusted."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.locations.withIncludedLocations

```ts
withIncludedLocations(includedLocations)
```

"A list of location IDs in scope of policy unless explicitly excluded. Can also be set to All, or AllTrusted."

### fn spec.initProvider.conditions.locations.withIncludedLocationsMixin

```ts
withIncludedLocationsMixin(includedLocations)
```

"A list of location IDs in scope of policy unless explicitly excluded. Can also be set to All, or AllTrusted."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.conditions.platforms

"A platforms block as documented below, which specifies platforms included in and excluded from the policy."

### fn spec.initProvider.conditions.platforms.withExcludedPlatforms

```ts
withExcludedPlatforms(excludedPlatforms)
```

"A list of platforms explicitly excluded from the policy. Possible values are: all, android, iOS, linux, macOS, windows, windowsPhone or unknownFutureValue."

### fn spec.initProvider.conditions.platforms.withExcludedPlatformsMixin

```ts
withExcludedPlatformsMixin(excludedPlatforms)
```

"A list of platforms explicitly excluded from the policy. Possible values are: all, android, iOS, linux, macOS, windows, windowsPhone or unknownFutureValue."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.platforms.withIncludedPlatforms

```ts
withIncludedPlatforms(includedPlatforms)
```

"A list of platforms the policy applies to, unless explicitly excluded. Possible values are: all, android, iOS, linux, macOS, windows, windowsPhone or unknownFutureValue."

### fn spec.initProvider.conditions.platforms.withIncludedPlatformsMixin

```ts
withIncludedPlatformsMixin(includedPlatforms)
```

"A list of platforms the policy applies to, unless explicitly excluded. Possible values are: all, android, iOS, linux, macOS, windows, windowsPhone or unknownFutureValue."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.conditions.users

"A users block as documented below, which specifies users, groups, and roles included in and excluded from the policy."

### fn spec.initProvider.conditions.users.withExcludedGroups

```ts
withExcludedGroups(excludedGroups)
```

"A list of group IDs excluded from scope of policy."

### fn spec.initProvider.conditions.users.withExcludedGroupsMixin

```ts
withExcludedGroupsMixin(excludedGroups)
```

"A list of group IDs excluded from scope of policy."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.users.withExcludedGuestsOrExternalUsers

```ts
withExcludedGuestsOrExternalUsers(excludedGuestsOrExternalUsers)
```

"A guests_or_external_users block as documented below, which specifies internal guests and external users excluded from scope of policy."

### fn spec.initProvider.conditions.users.withExcludedGuestsOrExternalUsersMixin

```ts
withExcludedGuestsOrExternalUsersMixin(excludedGuestsOrExternalUsers)
```

"A guests_or_external_users block as documented below, which specifies internal guests and external users excluded from scope of policy."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.users.withExcludedRoles

```ts
withExcludedRoles(excludedRoles)
```

"A list of role IDs excluded from scope of policy."

### fn spec.initProvider.conditions.users.withExcludedRolesMixin

```ts
withExcludedRolesMixin(excludedRoles)
```

"A list of role IDs excluded from scope of policy."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.users.withExcludedUsers

```ts
withExcludedUsers(excludedUsers)
```

"A list of user IDs excluded from scope of policy and/or GuestsOrExternalUsers."

### fn spec.initProvider.conditions.users.withExcludedUsersMixin

```ts
withExcludedUsersMixin(excludedUsers)
```

"A list of user IDs excluded from scope of policy and/or GuestsOrExternalUsers."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.users.withIncludedGroups

```ts
withIncludedGroups(includedGroups)
```

"A list of group IDs in scope of policy unless explicitly excluded."

### fn spec.initProvider.conditions.users.withIncludedGroupsMixin

```ts
withIncludedGroupsMixin(includedGroups)
```

"A list of group IDs in scope of policy unless explicitly excluded."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.users.withIncludedGuestsOrExternalUsers

```ts
withIncludedGuestsOrExternalUsers(includedGuestsOrExternalUsers)
```

"A guests_or_external_users block as documented below, which specifies internal guests and external users in scope of policy."

### fn spec.initProvider.conditions.users.withIncludedGuestsOrExternalUsersMixin

```ts
withIncludedGuestsOrExternalUsersMixin(includedGuestsOrExternalUsers)
```

"A guests_or_external_users block as documented below, which specifies internal guests and external users in scope of policy."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.users.withIncludedRoles

```ts
withIncludedRoles(includedRoles)
```

"A list of role IDs in scope of policy unless explicitly excluded."

### fn spec.initProvider.conditions.users.withIncludedRolesMixin

```ts
withIncludedRolesMixin(includedRoles)
```

"A list of role IDs in scope of policy unless explicitly excluded."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.users.withIncludedUsers

```ts
withIncludedUsers(includedUsers)
```

"A list of user IDs in scope of policy unless explicitly excluded, or None or All or GuestsOrExternalUsers."

### fn spec.initProvider.conditions.users.withIncludedUsersMixin

```ts
withIncludedUsersMixin(includedUsers)
```

"A list of user IDs in scope of policy unless explicitly excluded, or None or All or GuestsOrExternalUsers."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.conditions.users.excludedGuestsOrExternalUsers

"A guests_or_external_users block as documented below, which specifies internal guests and external users excluded from scope of policy."

### fn spec.initProvider.conditions.users.excludedGuestsOrExternalUsers.withExternalTenants

```ts
withExternalTenants(externalTenants)
```

"An external_tenants block as documented below, which specifies external tenants in a policy scope."

### fn spec.initProvider.conditions.users.excludedGuestsOrExternalUsers.withExternalTenantsMixin

```ts
withExternalTenantsMixin(externalTenants)
```

"An external_tenants block as documented below, which specifies external tenants in a policy scope."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.users.excludedGuestsOrExternalUsers.withGuestOrExternalUserTypes

```ts
withGuestOrExternalUserTypes(guestOrExternalUserTypes)
```

"A list of guest or external user types. Possible values are: b2bCollaborationGuest, b2bCollaborationMember, b2bDirectConnectUser, internalGuest, none, otherExternalUser, serviceProvider, unknownFutureValue."

### fn spec.initProvider.conditions.users.excludedGuestsOrExternalUsers.withGuestOrExternalUserTypesMixin

```ts
withGuestOrExternalUserTypesMixin(guestOrExternalUserTypes)
```

"A list of guest or external user types. Possible values are: b2bCollaborationGuest, b2bCollaborationMember, b2bDirectConnectUser, internalGuest, none, otherExternalUser, serviceProvider, unknownFutureValue."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.conditions.users.excludedGuestsOrExternalUsers.externalTenants

"An external_tenants block as documented below, which specifies external tenants in a policy scope."

### fn spec.initProvider.conditions.users.excludedGuestsOrExternalUsers.externalTenants.withMembers

```ts
withMembers(members)
```

"A list tenant IDs. Can only be specified if membership_kind is enumerated."

### fn spec.initProvider.conditions.users.excludedGuestsOrExternalUsers.externalTenants.withMembersMixin

```ts
withMembersMixin(members)
```

"A list tenant IDs. Can only be specified if membership_kind is enumerated."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.users.excludedGuestsOrExternalUsers.externalTenants.withMembershipKind

```ts
withMembershipKind(membershipKind)
```

"The external tenant membership kind. Possible values are: all, enumerated, unknownFutureValue."

## obj spec.initProvider.conditions.users.includedGuestsOrExternalUsers

"A guests_or_external_users block as documented below, which specifies internal guests and external users in scope of policy."

### fn spec.initProvider.conditions.users.includedGuestsOrExternalUsers.withExternalTenants

```ts
withExternalTenants(externalTenants)
```

"An external_tenants block as documented below, which specifies external tenants in a policy scope."

### fn spec.initProvider.conditions.users.includedGuestsOrExternalUsers.withExternalTenantsMixin

```ts
withExternalTenantsMixin(externalTenants)
```

"An external_tenants block as documented below, which specifies external tenants in a policy scope."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.users.includedGuestsOrExternalUsers.withGuestOrExternalUserTypes

```ts
withGuestOrExternalUserTypes(guestOrExternalUserTypes)
```

"A list of guest or external user types. Possible values are: b2bCollaborationGuest, b2bCollaborationMember, b2bDirectConnectUser, internalGuest, none, otherExternalUser, serviceProvider, unknownFutureValue."

### fn spec.initProvider.conditions.users.includedGuestsOrExternalUsers.withGuestOrExternalUserTypesMixin

```ts
withGuestOrExternalUserTypesMixin(guestOrExternalUserTypes)
```

"A list of guest or external user types. Possible values are: b2bCollaborationGuest, b2bCollaborationMember, b2bDirectConnectUser, internalGuest, none, otherExternalUser, serviceProvider, unknownFutureValue."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.conditions.users.includedGuestsOrExternalUsers.externalTenants

"An external_tenants block as documented below, which specifies external tenants in a policy scope."

### fn spec.initProvider.conditions.users.includedGuestsOrExternalUsers.externalTenants.withMembers

```ts
withMembers(members)
```

"A list tenant IDs. Can only be specified if membership_kind is enumerated."

### fn spec.initProvider.conditions.users.includedGuestsOrExternalUsers.externalTenants.withMembersMixin

```ts
withMembersMixin(members)
```

"A list tenant IDs. Can only be specified if membership_kind is enumerated."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.conditions.users.includedGuestsOrExternalUsers.externalTenants.withMembershipKind

```ts
withMembershipKind(membershipKind)
```

"The external tenant membership kind. Possible values are: all, enumerated, unknownFutureValue."

## obj spec.initProvider.grantControls

"A grant_controls block as documented below, which specifies the grant controls that must be fulfilled to pass the policy."

### fn spec.initProvider.grantControls.withAuthenticationStrengthPolicyId

```ts
withAuthenticationStrengthPolicyId(authenticationStrengthPolicyId)
```

"ID of an Authentication Strength Policy to use in this policy. When using a hard-coded ID, the UUID value should be prefixed with: /policies/authenticationStrengthPolicies/."

### fn spec.initProvider.grantControls.withBuiltInControls

```ts
withBuiltInControls(builtInControls)
```

"List of built-in controls required by the policy. Possible values are: block, mfa, approvedApplication, compliantApplication, compliantDevice, domainJoinedDevice, passwordChange or unknownFutureValue."

### fn spec.initProvider.grantControls.withBuiltInControlsMixin

```ts
withBuiltInControlsMixin(builtInControls)
```

"List of built-in controls required by the policy. Possible values are: block, mfa, approvedApplication, compliantApplication, compliantDevice, domainJoinedDevice, passwordChange or unknownFutureValue."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.grantControls.withCustomAuthenticationFactors

```ts
withCustomAuthenticationFactors(customAuthenticationFactors)
```

"List of custom controls IDs required by the policy."

### fn spec.initProvider.grantControls.withCustomAuthenticationFactorsMixin

```ts
withCustomAuthenticationFactorsMixin(customAuthenticationFactors)
```

"List of custom controls IDs required by the policy."

**Note:** This function appends passed data to existing values

### fn spec.initProvider.grantControls.withOperator

```ts
withOperator(operator)
```

"Defines the relationship of the grant controls. Possible values are: AND, OR."

### fn spec.initProvider.grantControls.withTermsOfUse

```ts
withTermsOfUse(termsOfUse)
```

"List of terms of use IDs required by the policy."

### fn spec.initProvider.grantControls.withTermsOfUseMixin

```ts
withTermsOfUseMixin(termsOfUse)
```

"List of terms of use IDs required by the policy."

**Note:** This function appends passed data to existing values

## obj spec.initProvider.sessionControls

"A session_controls block as documented below, which specifies the session controls that are enforced after sign-in."

### fn spec.initProvider.sessionControls.withApplicationEnforcedRestrictionsEnabled

```ts
withApplicationEnforcedRestrictionsEnabled(applicationEnforcedRestrictionsEnabled)
```

"Whether application enforced restrictions are enabled. Defaults to false."

### fn spec.initProvider.sessionControls.withCloudAppSecurityPolicy

```ts
withCloudAppSecurityPolicy(cloudAppSecurityPolicy)
```

"Enables cloud app security and specifies the cloud app security policy to use. Possible values are: blockDownloads, mcasConfigured, monitorOnly or unknownFutureValue."

### fn spec.initProvider.sessionControls.withDisableResilienceDefaults

```ts
withDisableResilienceDefaults(disableResilienceDefaults)
```

"Disables resilience defaults. Defaults to false."

### fn spec.initProvider.sessionControls.withPersistentBrowserMode

```ts
withPersistentBrowserMode(persistentBrowserMode)
```

"Session control to define whether to persist cookies. Possible values are: always or never."

### fn spec.initProvider.sessionControls.withSignInFrequency

```ts
withSignInFrequency(signInFrequency)
```

"Number of days or hours to enforce sign-in frequency. Required when sign_in_frequency_period is specified."

### fn spec.initProvider.sessionControls.withSignInFrequencyAuthenticationType

```ts
withSignInFrequencyAuthenticationType(signInFrequencyAuthenticationType)
```

"Authentication type for enforcing sign-in frequency. Possible values are: primaryAndSecondaryAuthentication or secondaryAuthentication. Defaults to primaryAndSecondaryAuthentication."

### fn spec.initProvider.sessionControls.withSignInFrequencyInterval

```ts
withSignInFrequencyInterval(signInFrequencyInterval)
```

"The interval to apply to sign-in frequency control. Possible values are: timeBased or everyTime. Defaults to timeBased."

### fn spec.initProvider.sessionControls.withSignInFrequencyPeriod

```ts
withSignInFrequencyPeriod(signInFrequencyPeriod)
```

"The time period to enforce sign-in frequency. Possible values are: hours or days. Required when sign_in_frequency_period is specified."

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