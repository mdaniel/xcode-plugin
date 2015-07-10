

# Introduction #

Creates build rules. Define compilers to be used for file types. Written in a file with the ending .xcbuildrules


# Parameters #

| `Name` | string | Name  |
|:-------|:-------|:------|
| `FileType` | string | Filetype identifier as defined in a FileTypeSpecification |
| `CompilerSpec` | string | Compiler identifier as defined in a CompilerSpecification |


# Example #

```
(
	{
		Name = "Erlang source rule";
		FileType = "sourcecode.erlang.erl";
		CompilerSpec = "org.erlang.compiler.erlc";
	},
)
```