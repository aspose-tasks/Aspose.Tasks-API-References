---
title: "MspDbSettings"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يسمح بتعيين الخيارات اللازمة لقراءة بيانات المشروع من قاعدة بيانات خادم MS Project."
type: docs
weight: 161
url: /ar/java/com.aspose.tasks/mspdbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MspDbSettings extends DbSettings
```

يسمح بتعيين الخيارات اللازمة لقراءة بيانات المشروع من قاعدة بيانات خادم MS Project.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [MspDbSettings(String connectionString, UUID projectGuid)](#MspDbSettings-java.lang.String-java.util.UUID-) | ينشئ مثيلاً جديداً من الفئة [MspDbSettings](../../com.aspose.tasks/mspdbsettings). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getProjectGuid()](#getProjectGuid--) | يحصل على guid الخاص بالمشروع للقراءة. |
| [getSchema()](#getSchema--) | يحصل على مخطط خادم MS Project. |
| [setSchema(String value)](#setSchema-java.lang.String-) | يضبط مخطط خادم MS Project. |
### MspDbSettings(String connectionString, UUID projectGuid) {#MspDbSettings-java.lang.String-java.util.UUID-}
```
public MspDbSettings(String connectionString, UUID projectGuid)
```


ينشئ مثيلاً جديداً من الفئة [MspDbSettings](../../com.aspose.tasks/mspdbsettings).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| connectionString | java.lang.String | سلسلة الاتصال المحددة. |
| projectGuid | java.util.UUID | guid المحدد لمشروع للقراءة. |

### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


يحصل على guid الخاص بالمشروع للقراءة.

**Returns:**
java.util.UUID - guid المشروع للقراءة.
### getSchema() {#getSchema--}
```
public final String getSchema()
```


يحصل على مخطط خادم MS Project. القيمة الافتراضية هي "pub".

**Returns:**
java.lang.String - مخطط خادم MS Project.
### setSchema(String value) {#setSchema-java.lang.String-}
```
public final void setSchema(String value)
```


يضبط مخطط خادم MS Project. القيمة الافتراضية هي "pub".

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | مخطط خادم MS Project. |

