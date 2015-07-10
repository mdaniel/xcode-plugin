# PBXTarget Class Reference #

---

**Inherits from** [PBXProjectItem](PBXProjectItem.md)

---

**Framework** `/Developer/Library/PrivateFrameworks/DevToolsCore.framework`

---


# Overview #

---

The `PBXTarget` class represents a low level binding to a target in a project.

# Adopted Protocols #

---

[XCCompatibilityChecking](XCCompatibilityChecking.md)
> [findFeaturesInUseAndAddToSet:usingPathPrefix:](XCProductPartOwners#findFeaturesInUseAndAddToSet:usingPathPrefix:.md)
[XCCompatibilityChecking](XCCompatibilityChecking.md)
> [createPropertyInfoContextWithBuildAction:configurationName:](XCCompatibilityChecking#createPropertyInfoContextWithBuildAction:configurationName.md)
> [configurationInspectionContextForConfigurationNamed:](XCCompatibilityChecking#configurationInspectionContextForConfigurationNamed:.md)
> [name](XCCompatibilityChecking#name.md)

# Tasks #

---


# Instance Methods #

---

## referenceWillBeRemoved: ##
`- (void)referenceWillBeRemoved:(id)arg1`
## referenceWasRenamed: ##
`- (void)referenceWasRenamed:(id)arg1`
## referenceWillChange: ##
`- (void)referenceWillChange:(id)arg1`
## referenceWasAdded: ##
`- (void)referenceWasAdded:(id)arg1`
## willChange ##
`- (void)willChange`
## untouchFileAtPath: ##
`- (void)untouchFileAtPath:(id)arg1`
## touchFileAtPath: ##
`- (void)touchFileAtPath:(id)arg1`
## fileMayHaveChangedAtPath: ##
`- (void)fileMayHaveChangedAtPath:(id)arg1`
## _unarchiverDidFinishUnarchiving: ##
`- (void)_unarchiverDidFinishUnarchiving:(id)arg1`
## awakeFromPListUnarchiver: ##
`- (void)awakeFromPListUnarchiver:(id)arg1`
## shouldArchiveProductSettingsXML ##
`- (BOOL)shouldArchiveProductSettingsXML`
##_createProductPartsFromProductTypeTemplateParts ##
`- (void)_createProductPartsFromProductTypeTemplateParts`
## subpartsForProductPart: ##
`- (id)subpartsForProductPart:(id)arg1`
## productPartForIdentifier: ##
`- (id)productPartForIdentifier:(id)arg1`
## productParts ##
`- (id)productParts`
## isJambased ##
`- (BOOL)isJambased`
## isNative ##
`- (BOOL)isNative`
## _infoPlistReferenceDidMove: ##
`- (void)_infoPlistReferenceDidMove:(id)arg1`
## infoPlistFilePath ##
`- (id)infoPlistFilePath`
## infoPlistFilePathForConfigurationNamed: ##
`- (id)infoPlistFilePathForConfigurationNamed:(id)arg1`
## fullProductNameForConfigurationNamed: ##
`- (id)fullProductNameForConfigurationNamed:(id)arg1`
## removeProductSettingForKey: ##
`- (void)removeProductSettingForKey:(id)arg1`
## setProductSetting:forKey: ##
`- (void)setProductSetting:(id)arg1 forKey:(id)arg2`
## productSettingForKey: ##
`- (id)productSettingForKey:(id)arg1`
## setProductSettings: ##
`- (void)setProductSettings:(id)arg1`
## productSettings ##
`- (id)productSettings`
## voidInfoPlistSettingsCache ##
`- (void)voidInfoPlistSettingsCache`
## productSettingsAreValid ##
`- (BOOL)productSettingsAreValid`
## writeOutInfoPlistSettings ##
`- (void)writeOutInfoPlistSettings`
##_writeOutInfoPlistSettingsUsing: ##
`- (void)_writeOutInfoPlistSettingsUsing:(id)arg1`
## setInfoPlistSettings: ##
`- (void)setInfoPlistSettings:(id)arg1`
## infoPlistSettings ##
`- (id)infoPlistSettings`
## intermediatesLocation ##
`- (id)intermediatesLocation`
## intermediatesLocationForConfigurationNamed: ##
`- (id)intermediatesLocationForConfigurationNamed:(id)arg1`
## builtProductsLocation ##
`- (id)builtProductsLocation`
## builtProductsLocationForConfigurationNamed: ##
`- (id)builtProductsLocationForConfigurationNamed:(id)arg1`
## dynamicallyComputedOverridingTargetBuildSettingsWithExpansionContext: ##
`- (id)dynamicallyComputedOverridingTargetBuildSettingsWithExpansionContext:(id)arg1`
## addBandIBuildSettingsToDynamicallyComputedTargetBuildSettings:withAction:andConfigurationName: ##
`- (void)addBandIBuildSettingsToDynamicallyComputedTargetBuildSettings:(id)arg1 withAction:(id)arg2 andConfigurationName:(id)arg3`
## relevantToolSpecifications ##
`- (id)relevantToolSpecifications`
## relevantToolSpecificationsForConfigurationsNamed: ##
`- (id)relevantToolSpecificationsForConfigurationsNamed:(id)arg1`
## relevantToolSpecificationsForConfigurationNamed: ##
`- (id)relevantToolSpecificationsForConfigurationNamed:(id)arg1`
## targetTypeDisplayName ##
`- (id)targetTypeDisplayName`
## canPackageHeaders ##
`- (BOOL)canPackageHeaders`
## canInstallHeaders ##
`- (BOOL)canInstallHeaders`
## wantsProductSettings ##
`- (BOOL)wantsProductSettings`
## hasUserConfigurableBuildRules ##
`- (BOOL)hasUserConfigurableBuildRules`
## productReferenceExpectedFileTypeForConfigurationNamed: ##
`- (id)productReferenceExpectedFileTypeForConfigurationNamed:(id)arg1`
## productReferenceIsExecutable ##
`- (BOOL)productReferenceIsExecutable`
## productTypeIdentifier: ##
`- (id)initWithName:(id)arg1 productTypeIdentifier:(id)arg2`
## baseDirectoryPath: ##
`- (id)initWithName:(id)arg1 productTypeIdentifier:(id)arg2 baseDirectoryPath:(id)arg3`
## 