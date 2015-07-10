# PBXContainerItem Class Reference #

---

**Inherits from** [PBXObject](PBXObject.md)

---

**Framework** `/Developer/Library/PrivateFrameworks/DevToolsCore.framework`

---


# Overview #

---

The `PBXContainerItem` class represents a low level binding to an item in a project that can reference contents.

# Adopted Protocols #

---

[PBXChangeNotification](PBXChangeNotification.md)
> [changeMask](PBXChangeNotification#changeMask.md)
> [willChangeWithArchivePriority:](PBXChangeNotification#willChangeWithArchivePriority:.md)
> [willChange](PBXChangeNotification#willChange.md)

# Class Methods #

---

## archiveNameForKey: ##
`+ (id)archiveNameForKey:(id)arg1`
## archivableUserAttributes ##
`+ (id)archivableUserAttributes`
## archivableAttributes ##
`+ (id)archivableAttributes`

# Instance Methods #

---

## shouldArchiveUserInterfaceContext ##
`- (BOOL)shouldArchiveUserInterfaceContext`
## shouldArchiveComments ##
`- (BOOL)shouldArchiveComments`
## removeObjectForUserInterfaceContextKey: ##
`- (void)removeObjectForUserInterfaceContextKey:(id)arg1`
## setObject:forUserInterfaceContextKey: ##
`- (void)setObject:(id)arg1 forUserInterfaceContextKey:(id)arg2`
## objectForUserInterfaceContextKey: ##
`- (id)objectForUserInterfaceContextKey:(id)arg1`
## setUserInterfaceContext: ##
`- (void)setUserInterfaceContext:(id)arg1`
## userInterfaceContext ##
`- (id)userInterfaceContext`
## willChangeWithArchivePriority: ##
`- (void)willChangeWithArchivePriority:(int)arg1`
## willChange ##
`- (void)willChange`
## changeMask ##
`- (int)changeMask`
## setContainer: ##
`- (void)setContainer:(id)arg1`
## container ##
`- (id)container`
## setProject: ##
`- (void)setProject:(id)arg1`
## project ##
`- (id)project`
## comments ##
`- (id)comments`
## setComments: ##
`- (void)setComments:(id)arg1`
## copyWithZone:getUnretainedObjectMappings: ##
`- (id)copyWithZone:(NSZone *)arg1 getUnretainedObjectMappings:(id *)arg2`
## init ##
`- (id)init`