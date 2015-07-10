

# Introduction #

Defines file types and their poperties. Written in a file with the ending .xcspec

# Parameters #

| `Type` | `"FileType"` | Required |
|:-------|:-------------|:---------|
| `Identifier` | string       | Unique Identifier  |
| `Name` | string       | Name of the filetype |
| `BasedOn` | string       | File type this is based on |
| `ComputerLanguage` | string       |          |
| `Language` | string       |          |
| `Class` | string       |          |

| `Extensions` | list | Extensions to recognize the file |
|:-------------|:-----|:---------------------------------|
| `MagicWord`  | list | Sting inside the file to recognize the file |
| `FilenamePatterns` | string | Regular expression to recognize the file |
| `MIMETypes`  | list |                                  |

| `IsExecutable` | bool | Is the file directly executable |
|:---------------|:-----|:--------------------------------|
| `RequiresHardTabs` | bool | Are soft tabs allowed           |
| `AppliesToBuildRules` | bool |                                 |
| `IsScannedForIncludes` | bool |                                 |
| `TypeCodes`    | list |                                 |
| `PlistStructureDefinition` | string |                                 |
| `ChangesCauseDependencyGraphInvalidation` | bool |                                 |
| `IsBuildPropertiesFile` | bool |                                 |
| `CanSetIncludeInIndex` | bool |                                 |
| `IncludeInIndex` | bool |                                 |
| `IsProjectWrapper` | bool |                                 |
| `IsStaticLibrary` | bool |                                 |
| `ContainsNativeCode` | bool |                                 |


# Example #

From the ASC Specifications
```
(
	{
		Type = FileType;
		Identifier = sourcecode.asc;
		BasedOn = sourcecode;
		Name = "ASC file";
		Extensions = (asc, lst);
		//ComputerLanguage = csharp;
		Language = "mono.lang.asc";
	}
)
```