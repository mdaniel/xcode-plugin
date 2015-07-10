

# Introduction #

Macros and snippets. Written in a file with the ending .xctxtmacro


# Parameters #

| `Identifier` | string | Unique Identifier for the macro |
|:-------------|:-------|:--------------------------------|
| `Name`       | string | Name of the macro               |
| `BasedOn `   | string | Unique Identifier of a parent macro  |
| `IsMenu`     | string | Is it a menu?                   |
| `IsMenuItem` | bool   | Is the macro visible in the menu? |
| `IncludeContexts` | list   | language context this macro is available in |
| `TextString` | string | The macro string itself ()      |
| `CompletionPrefix` | string |                                 |


# Example #

```
(
	{
		Identifier = erlang;
		Name = Erlang;
		IsMenu = YES;
		IncludeContexts = (
			"xcode.lang.erlang",
		);
	},
	{
		Identifier = "erlang.preprocessor";
		BasedOn = erlang;
		TextString = "-$(Tag)($(Contents)).";
	},
	{
		Identifier = "erlang.preprocessor.module";
		BasedOn = "erlang.preprocessor";
		Name = Module;
		IsMenuItem = YES;
		Tag = module;
		Contents = "<#!modulename!#>";
		CompletionPrefix = "module";
	},
	{
		Identifier = "erlang.preprocessor.author";
		BasedOn = "erlang.preprocessor";
		Name = Author;
		IsMenuItem = NO;
		Tag = author;
		Contents = "<#!author!#>";
		CompletionPrefix = "author";
	},
)
```