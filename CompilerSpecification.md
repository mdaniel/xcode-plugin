

# Introduction #

Defines compilers and their poperties.

**A LOT MORE NEEDED HERE**

# Parameters #

| `Type` | `"Compiler` | Required |
|:-------|:------------|:---------|
| `Identifier` | string      | Unique Identifier  |
| `Class` | string      |          |
| `Name` | string      | Name of the filetype |
| `Description` | string      |          |
| `Version` | string      |          |
| `Vendor` | string      |          |

| `ExecPath` | string | |
|:-----------|:-------|:|
| `OptionsForCommandLinePrefix` | string | |
| `Architectures` | list   | |
| `Languages` | list   | |
| `FileTypes` | list   | |

| `SupportsZeroLink` | bool | |
|:-------------------|:-----|:|
| `SupportsPredictiveCompilation` | bool | |
| `SupportsHeadermaps` | bool | |
| `CommandOutputParser` | list | see CommandOutputParser |
| `Options`          | dict | see below |
| `OptionCategories ` | dict | |

**Options dict:**
| `Name` | string | |
|:-------|:-------|:|
| `Type` | string | |
| `DefaultValue` | string | |
| `CommandLineArgs` | dict   | |
| `Category` | string | |
| `CommonOption` | string | |


# Example #

From the Erlang Compiler Specifications
```
(
{
	Type = Compiler;
	Identifier = "org.erlang.compiler.erlc";
	Class = "EXCompilerSpecificationErlc";
	Name = "Erlang Compiler";
	Description = "Erlang Compiler";
	Version = "R12B4";
	Vendor = "Erlang";
	ExecPath = "/usr/local/bin/erlc";
	OptionsForCommandLinePrefix = "ERLC_";
	Architectures = (
		beam,
		i386,
		ppc,
	);
	Languages = (
		erlang,
	);
	FileTypes = (
		"sourcecode.erlang.erl",
	);
	SupportsZeroLink = NO;
	SupportsPredictiveCompilation = NO;
	SupportsHeadermaps = NO;
	//CommandOutputParser = "EXCommandOutputParserErlc";
	CommandOutputParser = (
		("(.*?):([0-9]+): Warning:(.*)", emit-warning),
		("(.*?):([0-9]+): Error:(.*)", emit-error),
		("(.*?):([0-9]+): (.*)", emit-error)
	);
	Options = (
		{
			Name = "ERLC_OTHERFLAGS";
			Type = stringlist;
			DefaultValue = "";
			CommandLineArgs = {
				"" = ();
				"<<otherwise>>" = ("${0}");
			};
			Category = Language;
			CommonOption = NO;
		},
		{
			Name = "ERLC_OUTPUTDIR";
			Type = string;
			DefaultValue = ebin;
			CommandLineArgs = {
				"" = ();
				"<<otherwise>>" = ("-o${0}");
			};
			Category = Language;
			CommonOption = NO;
		},
	);
	OptionCategories = (
		{
			Name = Language;
			//IconName = "DX-option-language-d";
		},
	);
},
)
```