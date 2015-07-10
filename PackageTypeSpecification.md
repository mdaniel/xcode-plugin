

# Introduction #

Defines Package Types. Written in a file with the ending .xcspec

# Parameters #

| `Type` | `"PackageType"` | Required |
|:-------|:----------------|:---------|
| `Identifier` | string          | Unique Identifier  |
| `Name` | string          | Name of the package type |
| `Description` | string          |          |
| `BasedOn` | string          | package type  this is based on |

| `DefaultBuildSettings` | dict |  |
|:-----------------------|:-----|:-|
| `ProductReference`     | dict | see below dict |
| `HasInfoPlist`         | bool |  |
| `HasInfoPlistStrings`  | bool |  |

ProductReference dict:
| `FileType` | string |  |
|:-----------|:-------|:-|
| `Name`     | string |  |
| `IsLaunchable` | bool   |  |

# Example #

From `/Developer/Platforms/iPhoneOS.platform/Developer/Library/Xcode/Specifications/iPhoneOSPackageTypes.xcspec`
```
(
    // Application wrapper
    {   Type = PackageType;
        Identifier = com.apple.package-type.wrapper.application;
        BasedOn = com.apple.package-type.wrapper;
        Name = "Application Wrapper";
        Description = "Application Wrapper";
        DefaultBuildSettings = {
            GENERATE_PKGINFO_FILE = YES;
        };
        ProductReference = {
            FileType = wrapper.application;
            Name = "$(WRAPPER_NAME)";
            IsLaunchable = YES;
        };
    },

    // CFBundle wrapper
    {   Type = PackageType;
        Identifier = com.apple.package-type.wrapper;
        Name = "Wrapper";
        Description = "Wrapper";
        DefaultBuildSettings = {
            WRAPPER_PREFIX = "";
            WRAPPER_SUFFIX = ".bundle";
            WRAPPER_NAME = "$(WRAPPER_PREFIX)$(PRODUCT_NAME)$(WRAPPER_SUFFIX)";
            CONTENTS_FOLDER_PATH = "$(WRAPPER_NAME)";
            EXECUTABLE_PREFIX = "";
            EXECUTABLE_SUFFIX = "";
            EXECUTABLE_NAME = "$(EXECUTABLE_PREFIX)$(PRODUCT_NAME)$(EXECUTABLE_VARIANT_SUFFIX)$(EXECUTABLE_SUFFIX)";
            EXECUTABLE_FOLDER_PATH = "$(CONTENTS_FOLDER_PATH)";
            EXECUTABLE_PATH = "$(EXECUTABLE_FOLDER_PATH)/$(EXECUTABLE_NAME)";
            INFOPLIST_PATH = "$(CONTENTS_FOLDER_PATH)/Info.plist";
            INFOSTRINGS_PATH = "$(LOCALIZED_RESOURCES_FOLDER_PATH)/InfoPlist.strings";
            PKGINFO_PATH = "$(CONTENTS_FOLDER_PATH)/PkgInfo";
            OUTPUT_RESOURCE_RULES_PATH = "$(CONTENTS_FOLDER_PATH)/ResourceRules.plist";
            PBDEVELOPMENTPLIST_PATH = "$(CONTENTS_FOLDER_PATH)/pbdevelopment.plist";
            VERSIONPLIST_PATH = "$(CONTENTS_FOLDER_PATH)/version.plist";
            PUBLIC_HEADERS_FOLDER_PATH = "$(CONTENTS_FOLDER_PATH)/Headers";
            PRIVATE_HEADERS_FOLDER_PATH = "$(CONTENTS_FOLDER_PATH)/PrivateHeaders";
            EXECUTABLES_FOLDER_PATH = "$(CONTENTS_FOLDER_PATH)/Executables";
            FRAMEWORKS_FOLDER_PATH = "$(CONTENTS_FOLDER_PATH)/Frameworks";
            SHARED_FRAMEWORKS_FOLDER_PATH = "$(CONTENTS_FOLDER_PATH)/SharedFrameworks";
            SHARED_SUPPORT_FOLDER_PATH = "$(CONTENTS_FOLDER_PATH)/SharedSupport";
            UNLOCALIZED_RESOURCES_FOLDER_PATH = "$(CONTENTS_FOLDER_PATH)";
            DOCUMENTATION_FOLDER_PATH = "$(LOCALIZED_RESOURCES_FOLDER_PATH)/Documentation";
            PLUGINS_FOLDER_PATH = "$(CONTENTS_FOLDER_PATH)/PlugIns";
            SCRIPTS_FOLDER_PATH = "$(UNLOCALIZED_RESOURCES_FOLDER_PATH)/Scripts";
            JAVA_FOLDER_PATH = "$(UNLOCALIZED_RESOURCES_FOLDER_PATH)/Java";
        };
        ProductReference = {
            FileType = wrapper.cfbundle;
            Name = "$(WRAPPER_NAME)";
            IsLaunchable = NO;
        };
    },
)
```