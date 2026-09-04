---
title: "ProjectFileInfo"
second_title: "Aspose.Tasks for Java API 参考"
description: "该类实例包含有关项目文件格式以及创建该文件的 Microsoft Project 版本的信息。"
type: docs
weight: 222
url: /zh/java/com.aspose.tasks/projectfileinfo/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public final class ProjectFileInfo implements System.IEquatable<ProjectFileInfo>
```

该类实例包含有关项目文件格式以及创建该文件的 Microsoft Project 版本的信息。

--------------------

使用 CanRead 属性来定义库是否可以处理项目文件。
## 方法

| 方法 | 描述 |
| --- | --- |
| [canRead()](#canRead--) | 获取一个值，指示 Aspose.Tasks 是否可以处理项目文件。 |
| [equals(ProjectFileInfo other)](#equals-com.aspose.tasks.ProjectFileInfo-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 返回一个值，指示此实例是否等于指定的对象。 |
| [getProjectApplicationInfo()](#getProjectApplicationInfo--) | 获取项目文件的应用程序信息。 |
| [getProjectFileFormat()](#getProjectFileFormat--) | 获取项目文件的格式。 |
| [hashCode()](#hashCode--) | 返回 [ProjectFileInfo](../../com.aspose.tasks/projectfileinfo) 类实例的哈希码值。 |
| [isPasswordProtected()](#isPasswordProtected--) | 获取一个值，指示项目是否受密码保护。 |
### canRead() {#canRead--}
```
public final boolean canRead()
```


获取一个值，指示 Aspose.Tasks 是否可以处理项目文件。

**Returns:**
boolean - 表示是否可以 Aspose 的值。
### equals(ProjectFileInfo other) {#equals-com.aspose.tasks.ProjectFileInfo-}
```
public final boolean equals(ProjectFileInfo other)
```


返回一个值，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | [ProjectFileInfo](../../com.aspose.tasks/projectfileinfo) | 与此实例比较的指定对象。 |

**Returns:**
boolean - 如果指定的 ProjectFileInfo 与此实例具有相同的文件格式和应用程序信息，则返回 true。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


返回一个值，指示此实例是否等于指定的对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | 与此实例比较的指定对象。 |

**Returns:**
boolean - 如果指定的 ProjectFileInfo 与此实例具有相同的文件格式和应用程序信息，则返回 true。
### getProjectApplicationInfo() {#getProjectApplicationInfo--}
```
public final int getProjectApplicationInfo()
```


获取项目文件的应用程序信息。

**Returns:**
int - 项目文件的应用程序信息。
### getProjectFileFormat() {#getProjectFileFormat--}
```
public final int getProjectFileFormat()
```


获取项目文件的格式。

**Returns:**
int - 项目文件的格式。
### hashCode() {#hashCode--}
```
public int hashCode()
```


返回 [ProjectFileInfo](../../com.aspose.tasks/projectfileinfo) 类实例的哈希码值。

**Returns:**
int - 返回此对象的哈希码值。
### isPasswordProtected() {#isPasswordProtected--}
```
public final boolean isPasswordProtected()
```


获取一个值，指示项目是否受密码保护。

**Returns:**
boolean - 指示项目是否受密码保护的值。
