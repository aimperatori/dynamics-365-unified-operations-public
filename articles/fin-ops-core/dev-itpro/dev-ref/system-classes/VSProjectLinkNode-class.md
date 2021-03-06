---
title: VSProjectLinkNode class
description: This topic describes the VSProjectLinkNode class.
author: robinarh
manager: tonyafehr
ms.date: 06/25/2020
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-platform
ms.technology: 

audience: Developer
ms.reviewer: rhaertle
ms.search.scope: Operations
ms.search.region: Global
ms.author: rhaertle
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
---

# Class VSProjectLinkNode

[!include [banner](../../includes/banner.md)]

```xpp
class VSProjectLinkNode extends VSItemNode
```

The VSProjectLinkNode class represents links to other Application Object Tree (AOT) nodes in the Microsoft Visual Studio project nodes in the AOT.

## Remarks

## Examples

## Methods

| Method                                                             | Description                           |
|--------------------------------------------------------------------|---------------------------------------|
| public str AOTgetSource()                                          | Returns the source code of this node. |
| public str getAOTPath()                                            |                                       |
| public BinData getFileData()                                       |                                       |
| ::public static void notifyFileCreated(TreeNode node)              |                                       |
| public void setFile(str fileName)                                  |                                       |
| public void setFileData(BinData data)                              |                                       |
| public void getFile(str fileName)                                  |                                       |
| ::public static void notifyFileUpdated(TreeNode node)              |                                       |
| public void AOTsetSource(str source, \[boolean isStatic\])         | Sets the source code of this node.    |
| ::public static void notifyFileRenamed(TreeNode node, str oldName) |                                       |
| ::public static void notifyFileDeleted(TreeNode node, str aotPath) |                                       |

## Method AOTgetSource

Returns the source code of this node.

```xpp
public str AOTgetSource()
```

### Return Value - AOTgetSource

The string that contains source code, if there is any; otherwise, nullNothingnullptrunita null reference (Nothing in Visual Basic).

### Remarks - AOTgetSource

This function is overridden by nodes that have source code.

## Method getAOTPath

```xpp
public str getAOTPath()
```

### Return Value - getAOTPath

## Method getFileData

```xpp
public BinData getFileData()
```

### Return Value - getFileData

## Method notifyFileCreated

```xpp
public static void notifyFileCreated(TreeNode node)
```

### Parameters - notifyFileCreated

node  

## Method setFile

```xpp
public void setFile(str fileName)
```

### Parameters - setFile

fileName  

## Method setFileData

```xpp
public void setFileData(BinData data)
```

### Parameters - setFileData

data  

## Method getFile

```xpp
public void getFile(str fileName)
```

### Parameters - getFile

fileName  

## Method notifyFileUpdated

```xpp
public static void notifyFileUpdated(TreeNode node)
```

### Parameters - notifyFileUpdated

node  

## Method AOTsetSource

Sets the source code of this node.

```xpp
public void AOTsetSource(str source, [boolean isStatic])
```

### Parameters - AOTsetSource

source  
The value that specifies whether the method is static; optional.

<!-- -->

isStatic  
The value that specifies whether the method is static; optional.

### Remarks - AOTsetSource

This method is overridden by nodes that have source code.

## Method notifyFileRenamed

```xpp
public static void notifyFileRenamed(TreeNode node, str oldName)
```

### Parameters - notifyFileRenamed

node  

<!-- -->

oldName  

## Method notifyFileDeleted

```xpp
public static void notifyFileDeleted(TreeNode node, str aotPath)
```

### Parameters - notifyFileDeleted

node  

<!-- -->

aotPath  

