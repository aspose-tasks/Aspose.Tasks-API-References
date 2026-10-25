---
title: "PrimaveraBaseReader"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل قارئًا أساسيًا يمكن استخدامه لقراءة معرفات المشروع (UIDs) من ملفات Primavera XER أو XML متعددة المشاريع."
type: docs
weight: 196
url: /ar/java/com.aspose.tasks/primaverabasereader/
---

**Inheritance:**
java.lang.Object
```
public abstract class PrimaveraBaseReader
```

يمثل قارئًا أساسيًا يمكن استخدامه لقراءة معرفات المشروع (UIDs) من ملفات Primavera XER أو XML متعددة المشاريع.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getProjectInfos()](#getProjectInfos--) | إرجاع قائمة بكائنات معلومات مختصرة للمشروع. |
| [getProjectUids()](#getProjectUids--) | إرجاع قائمة بمعرفات فريدة للمشاريع. |
| [loadProject(int projectUid)](#loadProject-int-) | يقوم بتحميل المشروع بالمعرف الفريد المحدد. |
### getProjectInfos() {#getProjectInfos--}
```
public final List<PrimaveraProjectInfo> getProjectInfos()
```


إرجاع قائمة بكائنات معلومات مختصرة للمشروع.

**Returns:**
java.util.List&lt;com.aspose.tasks.PrimaveraProjectInfo&gt; - قائمة بكائنات معلومات مختصرة للمشروع
### getProjectUids() {#getProjectUids--}
```
public final List<Integer> getProjectUids()
```


إرجاع قائمة بمعرفات فريدة للمشاريع.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - قائمة بمعرفات فريدة للمشاريع.
### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


يقوم بتحميل المشروع بالمعرف الفريد المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| projectUid | int | معرّف فريد للمشروع الذي سيتم تحميله. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier from the specified multi project file. Null if project doesn't exist.
