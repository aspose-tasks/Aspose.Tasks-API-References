---
title: "MpdSettings"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يسمح بتعيين الخيارات الضرورية لقراءة بيانات المشروع من تنسيق MPD لملف قاعدة بيانات MS Access."
type: docs
weight: 160
url: /ar/java/com.aspose.tasks/mpdsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MpdSettings extends DbSettings
```

يسمح بتعيين الخيارات اللازمة لقراءة بيانات المشروع من تنسيق MPD (تنسيق ملف قاعدة بيانات MS Access).
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [MpdSettings(String connectionString, int projectId)](#MpdSettings-java.lang.String-int-) | يُهيئ مثيلًا جديدًا من الفئة `MpdSettings`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getProjectId()](#getProjectId--) | يعيد معرف المشروع للقراءة. |
### MpdSettings(String connectionString, int projectId) {#MpdSettings-java.lang.String-int-}
```
public MpdSettings(String connectionString, int projectId)
```


يُهيئ مثيلًا جديدًا من الفئة `MpdSettings`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| connectionString | java.lang.String | سلسلة الاتصال المحددة. |
| projectId | int | معرف المشروع المحدد للقراءة. |

### getProjectId() {#getProjectId--}
```
public int getProjectId()
```


يعيد معرف المشروع للقراءة.

**Returns:**
int - معرف المشروع للقراءة.
