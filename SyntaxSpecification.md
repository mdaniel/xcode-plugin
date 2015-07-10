

# Introduction #

Defines syntax types. Files have the ending .xcsynspec


# Parameters #

| `Identifier ` | string | Unique Identifier  |
|:--------------|:-------|:-------------------|
| `Name `       | string | Name               |
| `BasedOn`     | string | Unique Identifier of parent |
| `IncludeInPrefs ` | bool   |                    |
| `NameFormat ` | string |                    |
| `Color `      | string | default color      |
| `OldUserDefault ` | string | Only used by built in filetypes |



---


# Example #

From the D for XCode plugin
```
(
    {
        Identifier = "xcode.syntax.d.module";
        IncludeInPrefs = NO;
	NameFormat = "module %@";
    },
    {
        Identifier = "xcode.syntax.d.import";
        IncludeInPrefs = NO;
	NameFormat = "import %@";
    },
	
	// MARK: Functions and Methods
	{
		Identifier = "xcode.syntax.definition.d.function";
		BasedOn = "xcode.syntax.definition.function";
		IncludeInPrefs = NO;
	},
	{
		Identifier = "xcode.syntax.declaration.d.function";
		BasedOn = "xcode.syntax.declaration.function";
		IncludeInPrefs = NO;
	},
)
```