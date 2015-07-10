# PBXAbstractSCMScriptCommand Class Reference #

---

**Inherits from** NSObject

---

**Framework** `/Developer/Library/PrivateFrameworks/DevToolsCore.framework`

---


# Overview #

---

The `PBXAbstractSCMScriptCommand` class provides an interface for running source control commands via  a script.

# Tasks #

---

## Creating a PBXAbstractSCMScriptCommand Object ##
[- initWithCommandDescription:](#initWithCommandDescription:.md)

## Obtaining Return Values Object ##
[- returnValueFromInfo:](#returnValueFromInfo:.md)

[- returnScriptResultUsingInfo:](#returnScriptResultUsingInfo:.md)

## Requests ##
[- requestDidFinish:](#requestDidFinish:.md)

[- performRequestWithItems:onSCMManager:](#performRequestWithItems:onSCMManager:.md)

[- runCommandOnItems:inProject:](#runCommandOnItems:inProject:.md)

[- runCommandOnProject:](#runCommandOnProject:.md)

[- argumentsForRequest](#argumentsForRequest.md)

[- requestType](#requestType.md)

# Instance Methods #

---

## initWithCommandDescription: ##
`- (id)initWithCommandDescription:(id)arg1`
## returnValueFromInfo: ##
`- (id)returnValueFromInfo:(id)arg1`
## returnScriptResultUsingInfo: ##
`- (void)returnScriptResultUsingInfo:(id)arg1`
## requestDidFinish: ##
`- (void)requestDidFinish:(id)arg1`
## performRequestWithItems:onSCMManager ##
`- (id)performRequestWithItems:(id)arg1 onSCMManager:(id)arg2`
## runCommandOnItems:inProject: ##
`- (id)runCommandOnItems:(id)arg1 inProject:(id)arg2`
## runCommandOnProject ##
`- (id)runCommandOnProject:(id)arg1`
## argumentsForRequest ##
`- (id)argumentsForRequest`
## requestType ##
`- (id)requestType`