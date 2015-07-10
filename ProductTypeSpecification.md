

# Introduction #

Defines Product Types. Written in a file with the ending .xcspec

# Parameters #

| `Type` | `"ProductType"` | Required |
|:-------|:----------------|:---------|
| `Identifier` | string          | Unique Identifier  |
| `Name` | string          | Name of the product type |
| `Description` | string          |          |
| `BasedOn` | string          | product type  this is based on |
| `IconNamePrefix` | string          |          |
| `DefaultTargetName` | string          |          |
| `AllowedBuildPhaseTypes` | list            |          |
| `PackageTypes` | list            |          |

| `Class` | string |  |
|:--------|:-------|:-|
| `DefaultBuildProperties` | dict   |  |
| `IsWrapper` | bool   |  |
| `HasInfoPlist` | bool   |  |
| `HasInfoPlistStrings` | bool   |  |


# Example #

From `/Developer/Platforms/iPhoneOS.platform/Developer/Library/Xcode/Specifications/iPhoneOSProductTypes.xcspec`
```
(
    // Application
    {   Type = ProductType;
        Identifier = com.apple.product-type.application;
        BasedOn = com.apple.product-type.bundle;
        Class = PBXApplicationProductType;
        Name = "Application";
        Description = "Application";
        IconNamePrefix = "TargetApp";
        DefaultTargetName = "Application";
        SupportsZeroLink = YES;
        DefaultBuildProperties = {
            MACH_O_TYPE = "mh_execute";
            GCC_DYNAMIC_NO_PIC = YES;
            GCC_SYMBOLS_PRIVATE_EXTERN = YES;
            GCC_INLINES_ARE_PRIVATE_EXTERN = YES;
            WRAPPER_SUFFIX = ".$(WRAPPER_EXTENSION)";
            WRAPPER_EXTENSION = "app";
            INSTALL_PATH = "$(HOME)/Applications";
            STRIP_STYLE = "all";
            ENTITLEMENTS_ALLOWED = YES;
        };
        PackageTypes = (
            com.apple.package-type.wrapper.application
        );
    },
)
```