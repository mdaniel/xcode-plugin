# PBXAggregateTarget Class Reference #

---

**Inherits from** [PBXNativeTarget](PBXNativeTarget.md)

---

**Framework** `/Developer/Library/PrivateFrameworks/DevToolsCore.framework`

---


# Overview #

---

The `PBXAggregateTarget` class represents a low level binding to an aggregate target in a project.

# Tasks #

---


# Class Methods #

---

## standardBuildPhaseClasses ##
`+ (NSArray *)standardBuildPhaseClasses`
## targetTypeDisplayName ##
`+ (NSString *)targetTypeDisplayName`
## categorizedTargetName ##
`+ (NSString *)categorizedTargetName`

# Instance Methods #

---

## productReferenceExpectedFileTypeForConfigurationNamed: ##
`- (id)productReferenceExpectedFileTypeForConfigurationNamed:(id)arg1`
## productReferenceIsExecutable ##
`- (BOOL)productReferenceIsExecutable`
## relevantToolSpecifications ##
`- (id)relevantToolSpecifications`
## relevantToolSpecificationsForConfigurationsNamed: ##
`- (id)relevantToolSpecificationsForConfigurationsNamed:(id)arg1`
## relevantToolSpecificationsForConfigurationNamed: ##
`- (id)relevantToolSpecificationsForConfigurationNamed:(id)arg1`
## isAggregate ##
`- (BOOL)isAggregate`
## canPackageHeaders ##
`- (BOOL)canPackageHeaders`
## canInstallHeaders ##
`- (BOOL)canInstallHeaders`
## wantsProductSettings ##
`- (BOOL)wantsProductSettings`
## hasUserConfigurableBuildRules ##
`- (BOOL)hasUserConfigurableBuildRules`
## buildSettingsPanes ##
`- (id)buildSettingsPanes`
## defaultProductTypeIdentifierByAnalyzingConfiguration ##
`- (id)defaultProductTypeIdentifierByAnalyzingConfiguration`