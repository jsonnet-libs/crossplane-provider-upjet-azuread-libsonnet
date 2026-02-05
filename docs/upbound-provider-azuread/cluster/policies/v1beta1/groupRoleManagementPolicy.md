---
permalink: /upbound-provider-azuread/cluster/policies/v1beta1/groupRoleManagementPolicy/
---

# policies.v1beta1.groupRoleManagementPolicy

"GroupRoleManagementPolicy is the Schema for the GroupRoleManagementPolicys API."

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
    * [`fn withGroupId(groupId)`](#fn-specforproviderwithgroupid)
    * [`fn withRoleId(roleId)`](#fn-specforproviderwithroleid)
    * [`obj spec.forProvider.activationRules`](#obj-specforprovideractivationrules)
      * [`fn withMaximumDuration(maximumDuration)`](#fn-specforprovideractivationruleswithmaximumduration)
      * [`fn withRequireApproval(requireApproval)`](#fn-specforprovideractivationruleswithrequireapproval)
      * [`fn withRequireJustification(requireJustification)`](#fn-specforprovideractivationruleswithrequirejustification)
      * [`fn withRequireMultifactorAuthentication(requireMultifactorAuthentication)`](#fn-specforprovideractivationruleswithrequiremultifactorauthentication)
      * [`fn withRequireTicketInfo(requireTicketInfo)`](#fn-specforprovideractivationruleswithrequireticketinfo)
      * [`fn withRequiredConditionalAccessAuthenticationContext(requiredConditionalAccessAuthenticationContext)`](#fn-specforprovideractivationruleswithrequiredconditionalaccessauthenticationcontext)
      * [`obj spec.forProvider.activationRules.approvalStage`](#obj-specforprovideractivationrulesapprovalstage)
        * [`fn withPrimaryApprover(primaryApprover)`](#fn-specforprovideractivationrulesapprovalstagewithprimaryapprover)
        * [`fn withPrimaryApproverMixin(primaryApprover)`](#fn-specforprovideractivationrulesapprovalstagewithprimaryapprovermixin)
        * [`obj spec.forProvider.activationRules.approvalStage.primaryApprover`](#obj-specforprovideractivationrulesapprovalstageprimaryapprover)
          * [`fn withObjectId(objectId)`](#fn-specforprovideractivationrulesapprovalstageprimaryapproverwithobjectid)
          * [`fn withType(type)`](#fn-specforprovideractivationrulesapprovalstageprimaryapproverwithtype)
    * [`obj spec.forProvider.activeAssignmentRules`](#obj-specforprovideractiveassignmentrules)
      * [`fn withExpirationRequired(expirationRequired)`](#fn-specforprovideractiveassignmentruleswithexpirationrequired)
      * [`fn withExpireAfter(expireAfter)`](#fn-specforprovideractiveassignmentruleswithexpireafter)
      * [`fn withRequireJustification(requireJustification)`](#fn-specforprovideractiveassignmentruleswithrequirejustification)
      * [`fn withRequireMultifactorAuthentication(requireMultifactorAuthentication)`](#fn-specforprovideractiveassignmentruleswithrequiremultifactorauthentication)
      * [`fn withRequireTicketInfo(requireTicketInfo)`](#fn-specforprovideractiveassignmentruleswithrequireticketinfo)
    * [`obj spec.forProvider.eligibleAssignmentRules`](#obj-specforprovidereligibleassignmentrules)
      * [`fn withExpirationRequired(expirationRequired)`](#fn-specforprovidereligibleassignmentruleswithexpirationrequired)
      * [`fn withExpireAfter(expireAfter)`](#fn-specforprovidereligibleassignmentruleswithexpireafter)
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
    * [`obj spec.forProvider.notificationRules`](#obj-specforprovidernotificationrules)
      * [`obj spec.forProvider.notificationRules.activeAssignments`](#obj-specforprovidernotificationrulesactiveassignments)
        * [`obj spec.forProvider.notificationRules.activeAssignments.adminNotifications`](#obj-specforprovidernotificationrulesactiveassignmentsadminnotifications)
          * [`fn withAdditionalRecipients(additionalRecipients)`](#fn-specforprovidernotificationrulesactiveassignmentsadminnotificationswithadditionalrecipients)
          * [`fn withAdditionalRecipientsMixin(additionalRecipients)`](#fn-specforprovidernotificationrulesactiveassignmentsadminnotificationswithadditionalrecipientsmixin)
          * [`fn withDefaultRecipients(defaultRecipients)`](#fn-specforprovidernotificationrulesactiveassignmentsadminnotificationswithdefaultrecipients)
          * [`fn withNotificationLevel(notificationLevel)`](#fn-specforprovidernotificationrulesactiveassignmentsadminnotificationswithnotificationlevel)
        * [`obj spec.forProvider.notificationRules.activeAssignments.approverNotifications`](#obj-specforprovidernotificationrulesactiveassignmentsapprovernotifications)
          * [`fn withAdditionalRecipients(additionalRecipients)`](#fn-specforprovidernotificationrulesactiveassignmentsapprovernotificationswithadditionalrecipients)
          * [`fn withAdditionalRecipientsMixin(additionalRecipients)`](#fn-specforprovidernotificationrulesactiveassignmentsapprovernotificationswithadditionalrecipientsmixin)
          * [`fn withDefaultRecipients(defaultRecipients)`](#fn-specforprovidernotificationrulesactiveassignmentsapprovernotificationswithdefaultrecipients)
          * [`fn withNotificationLevel(notificationLevel)`](#fn-specforprovidernotificationrulesactiveassignmentsapprovernotificationswithnotificationlevel)
        * [`obj spec.forProvider.notificationRules.activeAssignments.assigneeNotifications`](#obj-specforprovidernotificationrulesactiveassignmentsassigneenotifications)
          * [`fn withAdditionalRecipients(additionalRecipients)`](#fn-specforprovidernotificationrulesactiveassignmentsassigneenotificationswithadditionalrecipients)
          * [`fn withAdditionalRecipientsMixin(additionalRecipients)`](#fn-specforprovidernotificationrulesactiveassignmentsassigneenotificationswithadditionalrecipientsmixin)
          * [`fn withDefaultRecipients(defaultRecipients)`](#fn-specforprovidernotificationrulesactiveassignmentsassigneenotificationswithdefaultrecipients)
          * [`fn withNotificationLevel(notificationLevel)`](#fn-specforprovidernotificationrulesactiveassignmentsassigneenotificationswithnotificationlevel)
      * [`obj spec.forProvider.notificationRules.eligibleActivations`](#obj-specforprovidernotificationruleseligibleactivations)
        * [`obj spec.forProvider.notificationRules.eligibleActivations.adminNotifications`](#obj-specforprovidernotificationruleseligibleactivationsadminnotifications)
          * [`fn withAdditionalRecipients(additionalRecipients)`](#fn-specforprovidernotificationruleseligibleactivationsadminnotificationswithadditionalrecipients)
          * [`fn withAdditionalRecipientsMixin(additionalRecipients)`](#fn-specforprovidernotificationruleseligibleactivationsadminnotificationswithadditionalrecipientsmixin)
          * [`fn withDefaultRecipients(defaultRecipients)`](#fn-specforprovidernotificationruleseligibleactivationsadminnotificationswithdefaultrecipients)
          * [`fn withNotificationLevel(notificationLevel)`](#fn-specforprovidernotificationruleseligibleactivationsadminnotificationswithnotificationlevel)
        * [`obj spec.forProvider.notificationRules.eligibleActivations.approverNotifications`](#obj-specforprovidernotificationruleseligibleactivationsapprovernotifications)
          * [`fn withAdditionalRecipients(additionalRecipients)`](#fn-specforprovidernotificationruleseligibleactivationsapprovernotificationswithadditionalrecipients)
          * [`fn withAdditionalRecipientsMixin(additionalRecipients)`](#fn-specforprovidernotificationruleseligibleactivationsapprovernotificationswithadditionalrecipientsmixin)
          * [`fn withDefaultRecipients(defaultRecipients)`](#fn-specforprovidernotificationruleseligibleactivationsapprovernotificationswithdefaultrecipients)
          * [`fn withNotificationLevel(notificationLevel)`](#fn-specforprovidernotificationruleseligibleactivationsapprovernotificationswithnotificationlevel)
        * [`obj spec.forProvider.notificationRules.eligibleActivations.assigneeNotifications`](#obj-specforprovidernotificationruleseligibleactivationsassigneenotifications)
          * [`fn withAdditionalRecipients(additionalRecipients)`](#fn-specforprovidernotificationruleseligibleactivationsassigneenotificationswithadditionalrecipients)
          * [`fn withAdditionalRecipientsMixin(additionalRecipients)`](#fn-specforprovidernotificationruleseligibleactivationsassigneenotificationswithadditionalrecipientsmixin)
          * [`fn withDefaultRecipients(defaultRecipients)`](#fn-specforprovidernotificationruleseligibleactivationsassigneenotificationswithdefaultrecipients)
          * [`fn withNotificationLevel(notificationLevel)`](#fn-specforprovidernotificationruleseligibleactivationsassigneenotificationswithnotificationlevel)
      * [`obj spec.forProvider.notificationRules.eligibleAssignments`](#obj-specforprovidernotificationruleseligibleassignments)
        * [`obj spec.forProvider.notificationRules.eligibleAssignments.adminNotifications`](#obj-specforprovidernotificationruleseligibleassignmentsadminnotifications)
          * [`fn withAdditionalRecipients(additionalRecipients)`](#fn-specforprovidernotificationruleseligibleassignmentsadminnotificationswithadditionalrecipients)
          * [`fn withAdditionalRecipientsMixin(additionalRecipients)`](#fn-specforprovidernotificationruleseligibleassignmentsadminnotificationswithadditionalrecipientsmixin)
          * [`fn withDefaultRecipients(defaultRecipients)`](#fn-specforprovidernotificationruleseligibleassignmentsadminnotificationswithdefaultrecipients)
          * [`fn withNotificationLevel(notificationLevel)`](#fn-specforprovidernotificationruleseligibleassignmentsadminnotificationswithnotificationlevel)
        * [`obj spec.forProvider.notificationRules.eligibleAssignments.approverNotifications`](#obj-specforprovidernotificationruleseligibleassignmentsapprovernotifications)
          * [`fn withAdditionalRecipients(additionalRecipients)`](#fn-specforprovidernotificationruleseligibleassignmentsapprovernotificationswithadditionalrecipients)
          * [`fn withAdditionalRecipientsMixin(additionalRecipients)`](#fn-specforprovidernotificationruleseligibleassignmentsapprovernotificationswithadditionalrecipientsmixin)
          * [`fn withDefaultRecipients(defaultRecipients)`](#fn-specforprovidernotificationruleseligibleassignmentsapprovernotificationswithdefaultrecipients)
          * [`fn withNotificationLevel(notificationLevel)`](#fn-specforprovidernotificationruleseligibleassignmentsapprovernotificationswithnotificationlevel)
        * [`obj spec.forProvider.notificationRules.eligibleAssignments.assigneeNotifications`](#obj-specforprovidernotificationruleseligibleassignmentsassigneenotifications)
          * [`fn withAdditionalRecipients(additionalRecipients)`](#fn-specforprovidernotificationruleseligibleassignmentsassigneenotificationswithadditionalrecipients)
          * [`fn withAdditionalRecipientsMixin(additionalRecipients)`](#fn-specforprovidernotificationruleseligibleassignmentsassigneenotificationswithadditionalrecipientsmixin)
          * [`fn withDefaultRecipients(defaultRecipients)`](#fn-specforprovidernotificationruleseligibleassignmentsassigneenotificationswithdefaultrecipients)
          * [`fn withNotificationLevel(notificationLevel)`](#fn-specforprovidernotificationruleseligibleassignmentsassigneenotificationswithnotificationlevel)
  * [`obj spec.initProvider`](#obj-specinitprovider)
    * [`fn withGroupId(groupId)`](#fn-specinitproviderwithgroupid)
    * [`fn withRoleId(roleId)`](#fn-specinitproviderwithroleid)
    * [`obj spec.initProvider.activationRules`](#obj-specinitprovideractivationrules)
      * [`fn withMaximumDuration(maximumDuration)`](#fn-specinitprovideractivationruleswithmaximumduration)
      * [`fn withRequireApproval(requireApproval)`](#fn-specinitprovideractivationruleswithrequireapproval)
      * [`fn withRequireJustification(requireJustification)`](#fn-specinitprovideractivationruleswithrequirejustification)
      * [`fn withRequireMultifactorAuthentication(requireMultifactorAuthentication)`](#fn-specinitprovideractivationruleswithrequiremultifactorauthentication)
      * [`fn withRequireTicketInfo(requireTicketInfo)`](#fn-specinitprovideractivationruleswithrequireticketinfo)
      * [`fn withRequiredConditionalAccessAuthenticationContext(requiredConditionalAccessAuthenticationContext)`](#fn-specinitprovideractivationruleswithrequiredconditionalaccessauthenticationcontext)
      * [`obj spec.initProvider.activationRules.approvalStage`](#obj-specinitprovideractivationrulesapprovalstage)
        * [`fn withPrimaryApprover(primaryApprover)`](#fn-specinitprovideractivationrulesapprovalstagewithprimaryapprover)
        * [`fn withPrimaryApproverMixin(primaryApprover)`](#fn-specinitprovideractivationrulesapprovalstagewithprimaryapprovermixin)
        * [`obj spec.initProvider.activationRules.approvalStage.primaryApprover`](#obj-specinitprovideractivationrulesapprovalstageprimaryapprover)
          * [`fn withObjectId(objectId)`](#fn-specinitprovideractivationrulesapprovalstageprimaryapproverwithobjectid)
          * [`fn withType(type)`](#fn-specinitprovideractivationrulesapprovalstageprimaryapproverwithtype)
    * [`obj spec.initProvider.activeAssignmentRules`](#obj-specinitprovideractiveassignmentrules)
      * [`fn withExpirationRequired(expirationRequired)`](#fn-specinitprovideractiveassignmentruleswithexpirationrequired)
      * [`fn withExpireAfter(expireAfter)`](#fn-specinitprovideractiveassignmentruleswithexpireafter)
      * [`fn withRequireJustification(requireJustification)`](#fn-specinitprovideractiveassignmentruleswithrequirejustification)
      * [`fn withRequireMultifactorAuthentication(requireMultifactorAuthentication)`](#fn-specinitprovideractiveassignmentruleswithrequiremultifactorauthentication)
      * [`fn withRequireTicketInfo(requireTicketInfo)`](#fn-specinitprovideractiveassignmentruleswithrequireticketinfo)
    * [`obj spec.initProvider.eligibleAssignmentRules`](#obj-specinitprovidereligibleassignmentrules)
      * [`fn withExpirationRequired(expirationRequired)`](#fn-specinitprovidereligibleassignmentruleswithexpirationrequired)
      * [`fn withExpireAfter(expireAfter)`](#fn-specinitprovidereligibleassignmentruleswithexpireafter)
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
    * [`obj spec.initProvider.notificationRules`](#obj-specinitprovidernotificationrules)
      * [`obj spec.initProvider.notificationRules.activeAssignments`](#obj-specinitprovidernotificationrulesactiveassignments)
        * [`obj spec.initProvider.notificationRules.activeAssignments.adminNotifications`](#obj-specinitprovidernotificationrulesactiveassignmentsadminnotifications)
          * [`fn withAdditionalRecipients(additionalRecipients)`](#fn-specinitprovidernotificationrulesactiveassignmentsadminnotificationswithadditionalrecipients)
          * [`fn withAdditionalRecipientsMixin(additionalRecipients)`](#fn-specinitprovidernotificationrulesactiveassignmentsadminnotificationswithadditionalrecipientsmixin)
          * [`fn withDefaultRecipients(defaultRecipients)`](#fn-specinitprovidernotificationrulesactiveassignmentsadminnotificationswithdefaultrecipients)
          * [`fn withNotificationLevel(notificationLevel)`](#fn-specinitprovidernotificationrulesactiveassignmentsadminnotificationswithnotificationlevel)
        * [`obj spec.initProvider.notificationRules.activeAssignments.approverNotifications`](#obj-specinitprovidernotificationrulesactiveassignmentsapprovernotifications)
          * [`fn withAdditionalRecipients(additionalRecipients)`](#fn-specinitprovidernotificationrulesactiveassignmentsapprovernotificationswithadditionalrecipients)
          * [`fn withAdditionalRecipientsMixin(additionalRecipients)`](#fn-specinitprovidernotificationrulesactiveassignmentsapprovernotificationswithadditionalrecipientsmixin)
          * [`fn withDefaultRecipients(defaultRecipients)`](#fn-specinitprovidernotificationrulesactiveassignmentsapprovernotificationswithdefaultrecipients)
          * [`fn withNotificationLevel(notificationLevel)`](#fn-specinitprovidernotificationrulesactiveassignmentsapprovernotificationswithnotificationlevel)
        * [`obj spec.initProvider.notificationRules.activeAssignments.assigneeNotifications`](#obj-specinitprovidernotificationrulesactiveassignmentsassigneenotifications)
          * [`fn withAdditionalRecipients(additionalRecipients)`](#fn-specinitprovidernotificationrulesactiveassignmentsassigneenotificationswithadditionalrecipients)
          * [`fn withAdditionalRecipientsMixin(additionalRecipients)`](#fn-specinitprovidernotificationrulesactiveassignmentsassigneenotificationswithadditionalrecipientsmixin)
          * [`fn withDefaultRecipients(defaultRecipients)`](#fn-specinitprovidernotificationrulesactiveassignmentsassigneenotificationswithdefaultrecipients)
          * [`fn withNotificationLevel(notificationLevel)`](#fn-specinitprovidernotificationrulesactiveassignmentsassigneenotificationswithnotificationlevel)
      * [`obj spec.initProvider.notificationRules.eligibleActivations`](#obj-specinitprovidernotificationruleseligibleactivations)
        * [`obj spec.initProvider.notificationRules.eligibleActivations.adminNotifications`](#obj-specinitprovidernotificationruleseligibleactivationsadminnotifications)
          * [`fn withAdditionalRecipients(additionalRecipients)`](#fn-specinitprovidernotificationruleseligibleactivationsadminnotificationswithadditionalrecipients)
          * [`fn withAdditionalRecipientsMixin(additionalRecipients)`](#fn-specinitprovidernotificationruleseligibleactivationsadminnotificationswithadditionalrecipientsmixin)
          * [`fn withDefaultRecipients(defaultRecipients)`](#fn-specinitprovidernotificationruleseligibleactivationsadminnotificationswithdefaultrecipients)
          * [`fn withNotificationLevel(notificationLevel)`](#fn-specinitprovidernotificationruleseligibleactivationsadminnotificationswithnotificationlevel)
        * [`obj spec.initProvider.notificationRules.eligibleActivations.approverNotifications`](#obj-specinitprovidernotificationruleseligibleactivationsapprovernotifications)
          * [`fn withAdditionalRecipients(additionalRecipients)`](#fn-specinitprovidernotificationruleseligibleactivationsapprovernotificationswithadditionalrecipients)
          * [`fn withAdditionalRecipientsMixin(additionalRecipients)`](#fn-specinitprovidernotificationruleseligibleactivationsapprovernotificationswithadditionalrecipientsmixin)
          * [`fn withDefaultRecipients(defaultRecipients)`](#fn-specinitprovidernotificationruleseligibleactivationsapprovernotificationswithdefaultrecipients)
          * [`fn withNotificationLevel(notificationLevel)`](#fn-specinitprovidernotificationruleseligibleactivationsapprovernotificationswithnotificationlevel)
        * [`obj spec.initProvider.notificationRules.eligibleActivations.assigneeNotifications`](#obj-specinitprovidernotificationruleseligibleactivationsassigneenotifications)
          * [`fn withAdditionalRecipients(additionalRecipients)`](#fn-specinitprovidernotificationruleseligibleactivationsassigneenotificationswithadditionalrecipients)
          * [`fn withAdditionalRecipientsMixin(additionalRecipients)`](#fn-specinitprovidernotificationruleseligibleactivationsassigneenotificationswithadditionalrecipientsmixin)
          * [`fn withDefaultRecipients(defaultRecipients)`](#fn-specinitprovidernotificationruleseligibleactivationsassigneenotificationswithdefaultrecipients)
          * [`fn withNotificationLevel(notificationLevel)`](#fn-specinitprovidernotificationruleseligibleactivationsassigneenotificationswithnotificationlevel)
      * [`obj spec.initProvider.notificationRules.eligibleAssignments`](#obj-specinitprovidernotificationruleseligibleassignments)
        * [`obj spec.initProvider.notificationRules.eligibleAssignments.adminNotifications`](#obj-specinitprovidernotificationruleseligibleassignmentsadminnotifications)
          * [`fn withAdditionalRecipients(additionalRecipients)`](#fn-specinitprovidernotificationruleseligibleassignmentsadminnotificationswithadditionalrecipients)
          * [`fn withAdditionalRecipientsMixin(additionalRecipients)`](#fn-specinitprovidernotificationruleseligibleassignmentsadminnotificationswithadditionalrecipientsmixin)
          * [`fn withDefaultRecipients(defaultRecipients)`](#fn-specinitprovidernotificationruleseligibleassignmentsadminnotificationswithdefaultrecipients)
          * [`fn withNotificationLevel(notificationLevel)`](#fn-specinitprovidernotificationruleseligibleassignmentsadminnotificationswithnotificationlevel)
        * [`obj spec.initProvider.notificationRules.eligibleAssignments.approverNotifications`](#obj-specinitprovidernotificationruleseligibleassignmentsapprovernotifications)
          * [`fn withAdditionalRecipients(additionalRecipients)`](#fn-specinitprovidernotificationruleseligibleassignmentsapprovernotificationswithadditionalrecipients)
          * [`fn withAdditionalRecipientsMixin(additionalRecipients)`](#fn-specinitprovidernotificationruleseligibleassignmentsapprovernotificationswithadditionalrecipientsmixin)
          * [`fn withDefaultRecipients(defaultRecipients)`](#fn-specinitprovidernotificationruleseligibleassignmentsapprovernotificationswithdefaultrecipients)
          * [`fn withNotificationLevel(notificationLevel)`](#fn-specinitprovidernotificationruleseligibleassignmentsapprovernotificationswithnotificationlevel)
        * [`obj spec.initProvider.notificationRules.eligibleAssignments.assigneeNotifications`](#obj-specinitprovidernotificationruleseligibleassignmentsassigneenotifications)
          * [`fn withAdditionalRecipients(additionalRecipients)`](#fn-specinitprovidernotificationruleseligibleassignmentsassigneenotificationswithadditionalrecipients)
          * [`fn withAdditionalRecipientsMixin(additionalRecipients)`](#fn-specinitprovidernotificationruleseligibleassignmentsassigneenotificationswithadditionalrecipientsmixin)
          * [`fn withDefaultRecipients(defaultRecipients)`](#fn-specinitprovidernotificationruleseligibleassignmentsassigneenotificationswithdefaultrecipients)
          * [`fn withNotificationLevel(notificationLevel)`](#fn-specinitprovidernotificationruleseligibleassignmentsassigneenotificationswithnotificationlevel)
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

new returns an instance of GroupRoleManagementPolicy

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

"GroupRoleManagementPolicySpec defines the desired state of GroupRoleManagementPolicy"

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



### fn spec.forProvider.withGroupId

```ts
withGroupId(groupId)
```

"The ID of the Azure AD group for which the policy applies.\nID of the group to which this policy is assigned"

### fn spec.forProvider.withRoleId

```ts
withRoleId(roleId)
```

"The type of assignment this policy coveres. Can be either member or owner.\nThe ID of the role of this policy to the group"

## obj spec.forProvider.activationRules

"An activation_rules block as defined below.\nThe activation rules of the policy"

### fn spec.forProvider.activationRules.withMaximumDuration

```ts
withMaximumDuration(maximumDuration)
```

"The maximum length of time an activated role can be valid, in an ISO8601 Duration format (e.g. PT8H). Valid range is PT30M to PT23H30M, in 30 minute increments, or PT1D.\nThe time after which the an activation can be valid for"

### fn spec.forProvider.activationRules.withRequireApproval

```ts
withRequireApproval(requireApproval)
```

"Is approval required for activation. If true an approval_stage block must be provided.\nWhether an approval is required for activation"

### fn spec.forProvider.activationRules.withRequireJustification

```ts
withRequireJustification(requireJustification)
```

"Is a justification required during activation of the role.\nWhether a justification is required during activation"

### fn spec.forProvider.activationRules.withRequireMultifactorAuthentication

```ts
withRequireMultifactorAuthentication(requireMultifactorAuthentication)
```

"Is multi-factor authentication required to activate the role. Conflicts with required_conditional_access_authentication_context.\nWhether multi-factor authentication is required during activation"

### fn spec.forProvider.activationRules.withRequireTicketInfo

```ts
withRequireTicketInfo(requireTicketInfo)
```

"Is ticket information requrired during activation of the role.\nWhether ticket information is required during activation"

### fn spec.forProvider.activationRules.withRequiredConditionalAccessAuthenticationContext

```ts
withRequiredConditionalAccessAuthenticationContext(requiredConditionalAccessAuthenticationContext)
```

"The Entra ID Conditional Access context that must be present for activation (e.g c1). Conflicts with require_multifactor_authentication.\nWhether a conditional access context is required during activation"

## obj spec.forProvider.activationRules.approvalStage

"An approval_stage block as defined below.\nThe approval stages for the activation"

### fn spec.forProvider.activationRules.approvalStage.withPrimaryApprover

```ts
withPrimaryApprover(primaryApprover)
```

"blocks as defined below.\nThe IDs of the users or groups who can approve the activation"

### fn spec.forProvider.activationRules.approvalStage.withPrimaryApproverMixin

```ts
withPrimaryApproverMixin(primaryApprover)
```

"blocks as defined below.\nThe IDs of the users or groups who can approve the activation"

**Note:** This function appends passed data to existing values

## obj spec.forProvider.activationRules.approvalStage.primaryApprover

"blocks as defined below.\nThe IDs of the users or groups who can approve the activation"

### fn spec.forProvider.activationRules.approvalStage.primaryApprover.withObjectId

```ts
withObjectId(objectId)
```

"The ID of the object which will act as an approver.\nThe ID of the object to act as an approver"

### fn spec.forProvider.activationRules.approvalStage.primaryApprover.withType

```ts
withType(type)
```

"The type of object acting as an approver. Possible options are singleUser and groupMembers.\nThe type of object acting as an approver"

## obj spec.forProvider.activeAssignmentRules

"An active_assignment_rules block as defined below.\nThe rules for active assignment of the policy"

### fn spec.forProvider.activeAssignmentRules.withExpirationRequired

```ts
withExpirationRequired(expirationRequired)
```

"Must an assignment have an expiry date. false allows permanent assignment.\nMust the assignment have an expiry date"

### fn spec.forProvider.activeAssignmentRules.withExpireAfter

```ts
withExpireAfter(expireAfter)
```

"The maximum length of time an assignment can be valid, as an ISO8601 duration. Permitted values: P15D, P30D, P90D, P180D, or P365D.\nThe duration after which assignments expire"

### fn spec.forProvider.activeAssignmentRules.withRequireJustification

```ts
withRequireJustification(requireJustification)
```

"Is a justification required to create new assignments.\nWhether a justification is required to make an assignment"

### fn spec.forProvider.activeAssignmentRules.withRequireMultifactorAuthentication

```ts
withRequireMultifactorAuthentication(requireMultifactorAuthentication)
```

"Is multi-factor authentication required to create new assignments.\nWhether multi-factor authentication is required to make an assignment"

### fn spec.forProvider.activeAssignmentRules.withRequireTicketInfo

```ts
withRequireTicketInfo(requireTicketInfo)
```

"Is ticket information required to create new assignments.\nWhether ticket information is required to make an assignment"

## obj spec.forProvider.eligibleAssignmentRules

"An eligible_assignment_rules block as defined below.\nThe rules for eligible assignment of the policy"

### fn spec.forProvider.eligibleAssignmentRules.withExpirationRequired

```ts
withExpirationRequired(expirationRequired)
```

"Must an assignment have an expiry date. false allows permanent assignment.\nMust the assignment have an expiry date"

### fn spec.forProvider.eligibleAssignmentRules.withExpireAfter

```ts
withExpireAfter(expireAfter)
```

"The maximum length of time an assignment can be valid, as an ISO8601 duration. Permitted values: P15D, P30D, P90D, P180D, or P365D.\nThe duration after which assignments expire"

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

## obj spec.forProvider.notificationRules

"A notification_rules block as defined below.\nThe notification rules of the policy"

## obj spec.forProvider.notificationRules.activeAssignments

"A notification_target block as defined below to configure notfications on active role assignments.\nNotifications about active assignments"

## obj spec.forProvider.notificationRules.activeAssignments.adminNotifications

"A notification_settings block as defined above.\nAdmin notification settings"

### fn spec.forProvider.notificationRules.activeAssignments.adminNotifications.withAdditionalRecipients

```ts
withAdditionalRecipients(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

### fn spec.forProvider.notificationRules.activeAssignments.adminNotifications.withAdditionalRecipientsMixin

```ts
withAdditionalRecipientsMixin(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.notificationRules.activeAssignments.adminNotifications.withDefaultRecipients

```ts
withDefaultRecipients(defaultRecipients)
```

"Should the default recipients receive these notifications.\nWhether the default recipients are notified"

### fn spec.forProvider.notificationRules.activeAssignments.adminNotifications.withNotificationLevel

```ts
withNotificationLevel(notificationLevel)
```

"What level of notifications should be sent. Options are All or Critical.\nWhat level of notifications are sent"

## obj spec.forProvider.notificationRules.activeAssignments.approverNotifications

"A notification_settings block as defined above.\nApprover notification settings"

### fn spec.forProvider.notificationRules.activeAssignments.approverNotifications.withAdditionalRecipients

```ts
withAdditionalRecipients(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

### fn spec.forProvider.notificationRules.activeAssignments.approverNotifications.withAdditionalRecipientsMixin

```ts
withAdditionalRecipientsMixin(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.notificationRules.activeAssignments.approverNotifications.withDefaultRecipients

```ts
withDefaultRecipients(defaultRecipients)
```

"Should the default recipients receive these notifications.\nWhether the default recipients are notified"

### fn spec.forProvider.notificationRules.activeAssignments.approverNotifications.withNotificationLevel

```ts
withNotificationLevel(notificationLevel)
```

"What level of notifications should be sent. Options are All or Critical.\nWhat level of notifications are sent"

## obj spec.forProvider.notificationRules.activeAssignments.assigneeNotifications

"A notification_settings block as defined above.\nAssignee notification settings"

### fn spec.forProvider.notificationRules.activeAssignments.assigneeNotifications.withAdditionalRecipients

```ts
withAdditionalRecipients(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

### fn spec.forProvider.notificationRules.activeAssignments.assigneeNotifications.withAdditionalRecipientsMixin

```ts
withAdditionalRecipientsMixin(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.notificationRules.activeAssignments.assigneeNotifications.withDefaultRecipients

```ts
withDefaultRecipients(defaultRecipients)
```

"Should the default recipients receive these notifications.\nWhether the default recipients are notified"

### fn spec.forProvider.notificationRules.activeAssignments.assigneeNotifications.withNotificationLevel

```ts
withNotificationLevel(notificationLevel)
```

"What level of notifications should be sent. Options are All or Critical.\nWhat level of notifications are sent"

## obj spec.forProvider.notificationRules.eligibleActivations

"A notification_target block as defined below for configuring notifications on activation of eligible role.\nNotifications about activations of eligible assignments"

## obj spec.forProvider.notificationRules.eligibleActivations.adminNotifications

"A notification_settings block as defined above.\nAdmin notification settings"

### fn spec.forProvider.notificationRules.eligibleActivations.adminNotifications.withAdditionalRecipients

```ts
withAdditionalRecipients(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

### fn spec.forProvider.notificationRules.eligibleActivations.adminNotifications.withAdditionalRecipientsMixin

```ts
withAdditionalRecipientsMixin(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.notificationRules.eligibleActivations.adminNotifications.withDefaultRecipients

```ts
withDefaultRecipients(defaultRecipients)
```

"Should the default recipients receive these notifications.\nWhether the default recipients are notified"

### fn spec.forProvider.notificationRules.eligibleActivations.adminNotifications.withNotificationLevel

```ts
withNotificationLevel(notificationLevel)
```

"What level of notifications should be sent. Options are All or Critical.\nWhat level of notifications are sent"

## obj spec.forProvider.notificationRules.eligibleActivations.approverNotifications

"A notification_settings block as defined above.\nApprover notification settings"

### fn spec.forProvider.notificationRules.eligibleActivations.approverNotifications.withAdditionalRecipients

```ts
withAdditionalRecipients(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

### fn spec.forProvider.notificationRules.eligibleActivations.approverNotifications.withAdditionalRecipientsMixin

```ts
withAdditionalRecipientsMixin(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.notificationRules.eligibleActivations.approverNotifications.withDefaultRecipients

```ts
withDefaultRecipients(defaultRecipients)
```

"Should the default recipients receive these notifications.\nWhether the default recipients are notified"

### fn spec.forProvider.notificationRules.eligibleActivations.approverNotifications.withNotificationLevel

```ts
withNotificationLevel(notificationLevel)
```

"What level of notifications should be sent. Options are All or Critical.\nWhat level of notifications are sent"

## obj spec.forProvider.notificationRules.eligibleActivations.assigneeNotifications

"A notification_settings block as defined above.\nAssignee notification settings"

### fn spec.forProvider.notificationRules.eligibleActivations.assigneeNotifications.withAdditionalRecipients

```ts
withAdditionalRecipients(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

### fn spec.forProvider.notificationRules.eligibleActivations.assigneeNotifications.withAdditionalRecipientsMixin

```ts
withAdditionalRecipientsMixin(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.notificationRules.eligibleActivations.assigneeNotifications.withDefaultRecipients

```ts
withDefaultRecipients(defaultRecipients)
```

"Should the default recipients receive these notifications.\nWhether the default recipients are notified"

### fn spec.forProvider.notificationRules.eligibleActivations.assigneeNotifications.withNotificationLevel

```ts
withNotificationLevel(notificationLevel)
```

"What level of notifications should be sent. Options are All or Critical.\nWhat level of notifications are sent"

## obj spec.forProvider.notificationRules.eligibleAssignments

"A notification_target block as defined below to configure notification on eligible role assignments.\nNotifications about eligible assignments"

## obj spec.forProvider.notificationRules.eligibleAssignments.adminNotifications

"A notification_settings block as defined above.\nAdmin notification settings"

### fn spec.forProvider.notificationRules.eligibleAssignments.adminNotifications.withAdditionalRecipients

```ts
withAdditionalRecipients(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

### fn spec.forProvider.notificationRules.eligibleAssignments.adminNotifications.withAdditionalRecipientsMixin

```ts
withAdditionalRecipientsMixin(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.notificationRules.eligibleAssignments.adminNotifications.withDefaultRecipients

```ts
withDefaultRecipients(defaultRecipients)
```

"Should the default recipients receive these notifications.\nWhether the default recipients are notified"

### fn spec.forProvider.notificationRules.eligibleAssignments.adminNotifications.withNotificationLevel

```ts
withNotificationLevel(notificationLevel)
```

"What level of notifications should be sent. Options are All or Critical.\nWhat level of notifications are sent"

## obj spec.forProvider.notificationRules.eligibleAssignments.approverNotifications

"A notification_settings block as defined above.\nApprover notification settings"

### fn spec.forProvider.notificationRules.eligibleAssignments.approverNotifications.withAdditionalRecipients

```ts
withAdditionalRecipients(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

### fn spec.forProvider.notificationRules.eligibleAssignments.approverNotifications.withAdditionalRecipientsMixin

```ts
withAdditionalRecipientsMixin(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.notificationRules.eligibleAssignments.approverNotifications.withDefaultRecipients

```ts
withDefaultRecipients(defaultRecipients)
```

"Should the default recipients receive these notifications.\nWhether the default recipients are notified"

### fn spec.forProvider.notificationRules.eligibleAssignments.approverNotifications.withNotificationLevel

```ts
withNotificationLevel(notificationLevel)
```

"What level of notifications should be sent. Options are All or Critical.\nWhat level of notifications are sent"

## obj spec.forProvider.notificationRules.eligibleAssignments.assigneeNotifications

"A notification_settings block as defined above.\nAssignee notification settings"

### fn spec.forProvider.notificationRules.eligibleAssignments.assigneeNotifications.withAdditionalRecipients

```ts
withAdditionalRecipients(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

### fn spec.forProvider.notificationRules.eligibleAssignments.assigneeNotifications.withAdditionalRecipientsMixin

```ts
withAdditionalRecipientsMixin(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

**Note:** This function appends passed data to existing values

### fn spec.forProvider.notificationRules.eligibleAssignments.assigneeNotifications.withDefaultRecipients

```ts
withDefaultRecipients(defaultRecipients)
```

"Should the default recipients receive these notifications.\nWhether the default recipients are notified"

### fn spec.forProvider.notificationRules.eligibleAssignments.assigneeNotifications.withNotificationLevel

```ts
withNotificationLevel(notificationLevel)
```

"What level of notifications should be sent. Options are All or Critical.\nWhat level of notifications are sent"

## obj spec.initProvider

"THIS IS A BETA FIELD. It will be honored\nunless the Management Policies feature flag is disabled.\nInitProvider holds the same fields as ForProvider, with the exception\nof Identifier and other resource reference fields. The fields that are\nin InitProvider are merged into ForProvider when the resource is created.\nThe same fields are also added to the terraform ignore_changes hook, to\navoid updating them after creation. This is useful for fields that are\nrequired on creation, but we do not desire to update them after creation,\nfor example because of an external controller is managing them, like an\nautoscaler."

### fn spec.initProvider.withGroupId

```ts
withGroupId(groupId)
```

"The ID of the Azure AD group for which the policy applies.\nID of the group to which this policy is assigned"

### fn spec.initProvider.withRoleId

```ts
withRoleId(roleId)
```

"The type of assignment this policy coveres. Can be either member or owner.\nThe ID of the role of this policy to the group"

## obj spec.initProvider.activationRules

"An activation_rules block as defined below.\nThe activation rules of the policy"

### fn spec.initProvider.activationRules.withMaximumDuration

```ts
withMaximumDuration(maximumDuration)
```

"The maximum length of time an activated role can be valid, in an ISO8601 Duration format (e.g. PT8H). Valid range is PT30M to PT23H30M, in 30 minute increments, or PT1D.\nThe time after which the an activation can be valid for"

### fn spec.initProvider.activationRules.withRequireApproval

```ts
withRequireApproval(requireApproval)
```

"Is approval required for activation. If true an approval_stage block must be provided.\nWhether an approval is required for activation"

### fn spec.initProvider.activationRules.withRequireJustification

```ts
withRequireJustification(requireJustification)
```

"Is a justification required during activation of the role.\nWhether a justification is required during activation"

### fn spec.initProvider.activationRules.withRequireMultifactorAuthentication

```ts
withRequireMultifactorAuthentication(requireMultifactorAuthentication)
```

"Is multi-factor authentication required to activate the role. Conflicts with required_conditional_access_authentication_context.\nWhether multi-factor authentication is required during activation"

### fn spec.initProvider.activationRules.withRequireTicketInfo

```ts
withRequireTicketInfo(requireTicketInfo)
```

"Is ticket information requrired during activation of the role.\nWhether ticket information is required during activation"

### fn spec.initProvider.activationRules.withRequiredConditionalAccessAuthenticationContext

```ts
withRequiredConditionalAccessAuthenticationContext(requiredConditionalAccessAuthenticationContext)
```

"The Entra ID Conditional Access context that must be present for activation (e.g c1). Conflicts with require_multifactor_authentication.\nWhether a conditional access context is required during activation"

## obj spec.initProvider.activationRules.approvalStage

"An approval_stage block as defined below.\nThe approval stages for the activation"

### fn spec.initProvider.activationRules.approvalStage.withPrimaryApprover

```ts
withPrimaryApprover(primaryApprover)
```

"blocks as defined below.\nThe IDs of the users or groups who can approve the activation"

### fn spec.initProvider.activationRules.approvalStage.withPrimaryApproverMixin

```ts
withPrimaryApproverMixin(primaryApprover)
```

"blocks as defined below.\nThe IDs of the users or groups who can approve the activation"

**Note:** This function appends passed data to existing values

## obj spec.initProvider.activationRules.approvalStage.primaryApprover

"blocks as defined below.\nThe IDs of the users or groups who can approve the activation"

### fn spec.initProvider.activationRules.approvalStage.primaryApprover.withObjectId

```ts
withObjectId(objectId)
```

"The ID of the object which will act as an approver.\nThe ID of the object to act as an approver"

### fn spec.initProvider.activationRules.approvalStage.primaryApprover.withType

```ts
withType(type)
```

"The type of object acting as an approver. Possible options are singleUser and groupMembers.\nThe type of object acting as an approver"

## obj spec.initProvider.activeAssignmentRules

"An active_assignment_rules block as defined below.\nThe rules for active assignment of the policy"

### fn spec.initProvider.activeAssignmentRules.withExpirationRequired

```ts
withExpirationRequired(expirationRequired)
```

"Must an assignment have an expiry date. false allows permanent assignment.\nMust the assignment have an expiry date"

### fn spec.initProvider.activeAssignmentRules.withExpireAfter

```ts
withExpireAfter(expireAfter)
```

"The maximum length of time an assignment can be valid, as an ISO8601 duration. Permitted values: P15D, P30D, P90D, P180D, or P365D.\nThe duration after which assignments expire"

### fn spec.initProvider.activeAssignmentRules.withRequireJustification

```ts
withRequireJustification(requireJustification)
```

"Is a justification required to create new assignments.\nWhether a justification is required to make an assignment"

### fn spec.initProvider.activeAssignmentRules.withRequireMultifactorAuthentication

```ts
withRequireMultifactorAuthentication(requireMultifactorAuthentication)
```

"Is multi-factor authentication required to create new assignments.\nWhether multi-factor authentication is required to make an assignment"

### fn spec.initProvider.activeAssignmentRules.withRequireTicketInfo

```ts
withRequireTicketInfo(requireTicketInfo)
```

"Is ticket information required to create new assignments.\nWhether ticket information is required to make an assignment"

## obj spec.initProvider.eligibleAssignmentRules

"An eligible_assignment_rules block as defined below.\nThe rules for eligible assignment of the policy"

### fn spec.initProvider.eligibleAssignmentRules.withExpirationRequired

```ts
withExpirationRequired(expirationRequired)
```

"Must an assignment have an expiry date. false allows permanent assignment.\nMust the assignment have an expiry date"

### fn spec.initProvider.eligibleAssignmentRules.withExpireAfter

```ts
withExpireAfter(expireAfter)
```

"The maximum length of time an assignment can be valid, as an ISO8601 duration. Permitted values: P15D, P30D, P90D, P180D, or P365D.\nThe duration after which assignments expire"

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

## obj spec.initProvider.notificationRules

"A notification_rules block as defined below.\nThe notification rules of the policy"

## obj spec.initProvider.notificationRules.activeAssignments

"A notification_target block as defined below to configure notfications on active role assignments.\nNotifications about active assignments"

## obj spec.initProvider.notificationRules.activeAssignments.adminNotifications

"A notification_settings block as defined above.\nAdmin notification settings"

### fn spec.initProvider.notificationRules.activeAssignments.adminNotifications.withAdditionalRecipients

```ts
withAdditionalRecipients(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

### fn spec.initProvider.notificationRules.activeAssignments.adminNotifications.withAdditionalRecipientsMixin

```ts
withAdditionalRecipientsMixin(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.notificationRules.activeAssignments.adminNotifications.withDefaultRecipients

```ts
withDefaultRecipients(defaultRecipients)
```

"Should the default recipients receive these notifications.\nWhether the default recipients are notified"

### fn spec.initProvider.notificationRules.activeAssignments.adminNotifications.withNotificationLevel

```ts
withNotificationLevel(notificationLevel)
```

"What level of notifications should be sent. Options are All or Critical.\nWhat level of notifications are sent"

## obj spec.initProvider.notificationRules.activeAssignments.approverNotifications

"A notification_settings block as defined above.\nApprover notification settings"

### fn spec.initProvider.notificationRules.activeAssignments.approverNotifications.withAdditionalRecipients

```ts
withAdditionalRecipients(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

### fn spec.initProvider.notificationRules.activeAssignments.approverNotifications.withAdditionalRecipientsMixin

```ts
withAdditionalRecipientsMixin(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.notificationRules.activeAssignments.approverNotifications.withDefaultRecipients

```ts
withDefaultRecipients(defaultRecipients)
```

"Should the default recipients receive these notifications.\nWhether the default recipients are notified"

### fn spec.initProvider.notificationRules.activeAssignments.approverNotifications.withNotificationLevel

```ts
withNotificationLevel(notificationLevel)
```

"What level of notifications should be sent. Options are All or Critical.\nWhat level of notifications are sent"

## obj spec.initProvider.notificationRules.activeAssignments.assigneeNotifications

"A notification_settings block as defined above.\nAssignee notification settings"

### fn spec.initProvider.notificationRules.activeAssignments.assigneeNotifications.withAdditionalRecipients

```ts
withAdditionalRecipients(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

### fn spec.initProvider.notificationRules.activeAssignments.assigneeNotifications.withAdditionalRecipientsMixin

```ts
withAdditionalRecipientsMixin(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.notificationRules.activeAssignments.assigneeNotifications.withDefaultRecipients

```ts
withDefaultRecipients(defaultRecipients)
```

"Should the default recipients receive these notifications.\nWhether the default recipients are notified"

### fn spec.initProvider.notificationRules.activeAssignments.assigneeNotifications.withNotificationLevel

```ts
withNotificationLevel(notificationLevel)
```

"What level of notifications should be sent. Options are All or Critical.\nWhat level of notifications are sent"

## obj spec.initProvider.notificationRules.eligibleActivations

"A notification_target block as defined below for configuring notifications on activation of eligible role.\nNotifications about activations of eligible assignments"

## obj spec.initProvider.notificationRules.eligibleActivations.adminNotifications

"A notification_settings block as defined above.\nAdmin notification settings"

### fn spec.initProvider.notificationRules.eligibleActivations.adminNotifications.withAdditionalRecipients

```ts
withAdditionalRecipients(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

### fn spec.initProvider.notificationRules.eligibleActivations.adminNotifications.withAdditionalRecipientsMixin

```ts
withAdditionalRecipientsMixin(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.notificationRules.eligibleActivations.adminNotifications.withDefaultRecipients

```ts
withDefaultRecipients(defaultRecipients)
```

"Should the default recipients receive these notifications.\nWhether the default recipients are notified"

### fn spec.initProvider.notificationRules.eligibleActivations.adminNotifications.withNotificationLevel

```ts
withNotificationLevel(notificationLevel)
```

"What level of notifications should be sent. Options are All or Critical.\nWhat level of notifications are sent"

## obj spec.initProvider.notificationRules.eligibleActivations.approverNotifications

"A notification_settings block as defined above.\nApprover notification settings"

### fn spec.initProvider.notificationRules.eligibleActivations.approverNotifications.withAdditionalRecipients

```ts
withAdditionalRecipients(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

### fn spec.initProvider.notificationRules.eligibleActivations.approverNotifications.withAdditionalRecipientsMixin

```ts
withAdditionalRecipientsMixin(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.notificationRules.eligibleActivations.approverNotifications.withDefaultRecipients

```ts
withDefaultRecipients(defaultRecipients)
```

"Should the default recipients receive these notifications.\nWhether the default recipients are notified"

### fn spec.initProvider.notificationRules.eligibleActivations.approverNotifications.withNotificationLevel

```ts
withNotificationLevel(notificationLevel)
```

"What level of notifications should be sent. Options are All or Critical.\nWhat level of notifications are sent"

## obj spec.initProvider.notificationRules.eligibleActivations.assigneeNotifications

"A notification_settings block as defined above.\nAssignee notification settings"

### fn spec.initProvider.notificationRules.eligibleActivations.assigneeNotifications.withAdditionalRecipients

```ts
withAdditionalRecipients(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

### fn spec.initProvider.notificationRules.eligibleActivations.assigneeNotifications.withAdditionalRecipientsMixin

```ts
withAdditionalRecipientsMixin(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.notificationRules.eligibleActivations.assigneeNotifications.withDefaultRecipients

```ts
withDefaultRecipients(defaultRecipients)
```

"Should the default recipients receive these notifications.\nWhether the default recipients are notified"

### fn spec.initProvider.notificationRules.eligibleActivations.assigneeNotifications.withNotificationLevel

```ts
withNotificationLevel(notificationLevel)
```

"What level of notifications should be sent. Options are All or Critical.\nWhat level of notifications are sent"

## obj spec.initProvider.notificationRules.eligibleAssignments

"A notification_target block as defined below to configure notification on eligible role assignments.\nNotifications about eligible assignments"

## obj spec.initProvider.notificationRules.eligibleAssignments.adminNotifications

"A notification_settings block as defined above.\nAdmin notification settings"

### fn spec.initProvider.notificationRules.eligibleAssignments.adminNotifications.withAdditionalRecipients

```ts
withAdditionalRecipients(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

### fn spec.initProvider.notificationRules.eligibleAssignments.adminNotifications.withAdditionalRecipientsMixin

```ts
withAdditionalRecipientsMixin(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.notificationRules.eligibleAssignments.adminNotifications.withDefaultRecipients

```ts
withDefaultRecipients(defaultRecipients)
```

"Should the default recipients receive these notifications.\nWhether the default recipients are notified"

### fn spec.initProvider.notificationRules.eligibleAssignments.adminNotifications.withNotificationLevel

```ts
withNotificationLevel(notificationLevel)
```

"What level of notifications should be sent. Options are All or Critical.\nWhat level of notifications are sent"

## obj spec.initProvider.notificationRules.eligibleAssignments.approverNotifications

"A notification_settings block as defined above.\nApprover notification settings"

### fn spec.initProvider.notificationRules.eligibleAssignments.approverNotifications.withAdditionalRecipients

```ts
withAdditionalRecipients(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

### fn spec.initProvider.notificationRules.eligibleAssignments.approverNotifications.withAdditionalRecipientsMixin

```ts
withAdditionalRecipientsMixin(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.notificationRules.eligibleAssignments.approverNotifications.withDefaultRecipients

```ts
withDefaultRecipients(defaultRecipients)
```

"Should the default recipients receive these notifications.\nWhether the default recipients are notified"

### fn spec.initProvider.notificationRules.eligibleAssignments.approverNotifications.withNotificationLevel

```ts
withNotificationLevel(notificationLevel)
```

"What level of notifications should be sent. Options are All or Critical.\nWhat level of notifications are sent"

## obj spec.initProvider.notificationRules.eligibleAssignments.assigneeNotifications

"A notification_settings block as defined above.\nAssignee notification settings"

### fn spec.initProvider.notificationRules.eligibleAssignments.assigneeNotifications.withAdditionalRecipients

```ts
withAdditionalRecipients(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

### fn spec.initProvider.notificationRules.eligibleAssignments.assigneeNotifications.withAdditionalRecipientsMixin

```ts
withAdditionalRecipientsMixin(additionalRecipients)
```

"A list of additional email addresses that will receive these notifications.\nThe additional recipients to notify"

**Note:** This function appends passed data to existing values

### fn spec.initProvider.notificationRules.eligibleAssignments.assigneeNotifications.withDefaultRecipients

```ts
withDefaultRecipients(defaultRecipients)
```

"Should the default recipients receive these notifications.\nWhether the default recipients are notified"

### fn spec.initProvider.notificationRules.eligibleAssignments.assigneeNotifications.withNotificationLevel

```ts
withNotificationLevel(notificationLevel)
```

"What level of notifications should be sent. Options are All or Critical.\nWhat level of notifications are sent"

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