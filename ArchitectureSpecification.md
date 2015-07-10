

# Introduction #

> Defines Architectures. Written in a file with the ending .xcspec

# Parameters #

| `Type` | `"Architecture"` | Required |
|:-------|:-----------------|:---------|
| `Identifier` | string           | Unique Identifier  |
| `Name` | string           | Name of the filetype |
| `Description` | string           |          |
| `ListInEnum` | bool             |          |
| `SortNumber` | int              |          |
| `RealArchitectures` | list             |          |
| `ArchitectureSetting` | string           |          |

| `PerArchBuildSettingName` | string |  |
|:--------------------------|:-------|:-|
| `ByteOrder`               | int    |  |




# Example #

From `Developer/Platforms/iPhoneOS.platform/Developer/Library/Xcode/Specifications/iPhoneOSArchitectures.xcspec`
```
(
    {   Type = Architecture;
        Identifier = PlatformStandard;
        Name = "Standard (iPhone OS: armv6)";
        Description = "32-bit ARMv6 architecture";
        ListInEnum = YES;
        SortNumber = 1;
        RealArchitectures = ( armv6 );
        ArchitectureSetting = "ARCHS_STANDARD_32_BIT";
    },
    {   Type = Architecture;
        Identifier = Platform64bit;
        Name = "Standard 32/64-bit (iPhone OS: armv6)";
        Description = "32- and 64-bit ARMv6 architecture";
        ListInEnum = NO;
        SortNumber = 2;
        RealArchitectures = ( armv6 );
        ArchitectureSetting = "ARCHS_STANDARD_32_64_BIT";
    },
    // ARMv6
    {   Type = Architecture;
        Identifier = armv6;
        Name = "ARMv6";
        Description = "ARMv6";
        PerArchBuildSettingName = "ARMv6";
        ByteOrder = little;
        SortNumber = 100;
    },
)
```