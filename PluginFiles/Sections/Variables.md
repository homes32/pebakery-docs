# Plugin [Variables] Section

This section contains any pre-defined variables and macros the plugin needs to reference. The variables are loaded into memory when the plugin is processed during a build, a section within the plugin is called using the `Exec` command, or when another plugin loads them with the `AddVariables` command.

## Syntax

Plugin variables and macros are defined using the .INI style `Key=Value` format. Variables must be enclosed in `%` percent signs.

### Variables
```pebakery
%myProgramName%="My Program"
```

### Macros
```pebakery
myMacro=Run,%PluginFile%,DoSomething
```

## Remarks

None.

## Related

[AddVariables](/Commands/Control/AddVariables.md), [Variables](), [Macros](), [Exec](/Commands/Branch/Exec.md)

## Examples

### Example 1

```pebakery
[Main]
Title=Vairables Section
Description=Variables Section Example
Author=Homes32
Level=5
Version=1

[Variables]
%myProgramName%="My Program"
myMacro=Run,%PluginFile%,EchoMessage

[Process]
myMacro,%myProgramName%

[EchoMessage]
Echo,#1
Message,#1
```

