---
title: "PrimaveraDbReader"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل قارئًا لقراءة معلومات المشروع من قاعدة بيانات Primavera."
type: docs
weight: 200
url: /ar/java/com.aspose.tasks/primaveradbreader/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.PrimaveraBaseReader](../../com.aspose.tasks/primaverabasereader)
```
public final class PrimaveraDbReader extends PrimaveraBaseReader
```

يمثل قارئًا لقراءة معلومات المشروع من قاعدة بيانات Primavera.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PrimaveraDbReader(PrimaveraDbSettings dbSettings)](#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-) | ينشئ مثيلًا جديدًا من الفئة [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [loadProject(int projectUid)](#loadProject-int-) | يقوم بتحميل المشروع بالمعرف الفريد المحدد. |
### PrimaveraDbReader(PrimaveraDbSettings dbSettings) {#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-}
```
public PrimaveraDbReader(PrimaveraDbSettings dbSettings)
```


ينشئ مثيلًا جديدًا من الفئة [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| dbSettings | [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) | الإعدادات التي تحدد كيفية الاتصال بقاعدة بيانات Primavera. |

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
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier read from Primavera DB. Null if project doesn't exist.
