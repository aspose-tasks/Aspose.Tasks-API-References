---
title: "ProjectServerSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يسمح بتحديد خيارات إضافية عند حفظ المشروع إلى Project Server أو Project Online."
type: docs
weight: 227
url: /ar/java/com.aspose.tasks/projectserversaveoptions/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerSaveOptions
```

يسمح بتحديد خيارات إضافية عند حفظ المشروع إلى Project Server أو Project Online.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ProjectServerSaveOptions()](#ProjectServerSaveOptions--) | ينشئ مثيلاً جديداً من الفئة [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getPollingInterval()](#getPollingInterval--) | يحصل على الفاصل الزمني بين طلبات حالة وظائف الطابور. |
| [getProjectGuid()](#getProjectGuid--) | يحصل على المعرف الفريد لمشروع. |
| [getProjectName()](#getProjectName--) | يحصل على اسم المشروع الذي يُعرض في قائمة مشاريع Project Server \\\\ Project Online. |
| [getTimeout()](#getTimeout--) | يحصل على مهلة الانتظار المستخدمة عند انتظار معالجة طلب حفظ المشروع بواسطة خدمة معالجة طابور Project Server. |
| [setPollingInterval(double value)](#setPollingInterval-double-) | يضبط الفاصل الزمني بين طلبات حالة وظائف الطابور. |
| [setProjectGuid(UUID value)](#setProjectGuid-java.util.UUID-) | يضبط المعرف الفريد لمشروع. |
| [setProjectName(String value)](#setProjectName-java.lang.String-) | يضبط اسم المشروع الذي يُعرض في قائمة مشاريع Project Server \\\\ Project Online. |
| [setTimeout(double value)](#setTimeout-double-) | يضبط مهلة الانتظار المستخدمة عند انتظار معالجة طلب حفظ المشروع بواسطة خدمة معالجة طابور Project Server. |
### ProjectServerSaveOptions() {#ProjectServerSaveOptions--}
```
public ProjectServerSaveOptions()
```


ينشئ مثيلاً جديداً من الفئة [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions).

### getPollingInterval() {#getPollingInterval--}
```
public final double getPollingInterval()
```


يحصل على الفاصل الزمني بين طلبات حالة وظائف الطابور. القيمة الافتراضية هي 2 ثانية.

**Returns:**
double - الفاصل الزمني بين طلبات حالة وظائف الطابور.
### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


يحصل على المعرف الفريد لمشروع. يجب أن يكون فريداً داخل مثيل Project Server \\\\ Project Online.

**Returns:**
java.util.UUID - المعرف الفريد لمشروع.
### getProjectName() {#getProjectName--}
```
public final String getProjectName()
```


يحصل على اسم المشروع الذي يُعرض في قائمة مشاريع Project Server \\\\ Project Online. يجب أن يكون فريداً داخل مثيل Project Server \\\\ Project Online. إذا تم حذف القيمة، سيتم استخدام قيمة خاصية Prj.Name بدلاً منها.

**Returns:**
java.lang.String - اسم المشروع الذي يُعرض في قائمة مشاريع Project Server \\\\ Project Online.
### getTimeout() {#getTimeout--}
```
public final double getTimeout()
```


يحصل على مهلة الانتظار المستخدمة عند انتظار معالجة طلب حفظ المشروع بواسطة خدمة معالجة طابور Project Server. القيمة الافتراضية لهذه الخاصية هي دقيقة واحدة.

--------------------

قد يكون وقت المعالجة أطول للمشروعات الكبيرة أو في حالة عندما يكون مثيل خادم المشروع مشغولًا جدًا في الاستجابة للطلبات الأخرى.

**Returns:**
double - مهلة الانتظار المستخدمة عند انتظار معالجة طلب حفظ المشروع بواسطة خدمة معالجة طابور خادم المشروع.
### setPollingInterval(double value) {#setPollingInterval-double-}
```
public final void setPollingInterval(double value)
```


يضبط الفاصل الزمني بين طلبات حالة وظائف الطابور. القيمة الافتراضية هي ثانيتان.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | الفاصل الزمني بين طلبات حالة وظائف الطابور. |

### setProjectGuid(UUID value) {#setProjectGuid-java.util.UUID-}
```
public final void setProjectGuid(UUID value)
```


يضبط المعرف الفريد للمشروع. يجب أن يكون فريدًا داخل مثيل خادم المشروع \\ مشروع أونلاين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.UUID | المعرف الفريد للمشروع. |

### setProjectName(String value) {#setProjectName-java.lang.String-}
```
public final void setProjectName(String value)
```


يضبط اسم المشروع الذي يُعرض في قائمة مشاريع خادم المشروع \\ مشروع أونلاين. يجب أن يكون فريدًا داخل مثيل خادم المشروع \\ مشروع أونلاين. إذا تم حذف القيمة، سيتم استخدام قيمة خاصية Prj.Name بدلاً من ذلك.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | اسم المشروع الذي يُعرض في قائمة مشاريع خادم المشروع \\ مشروع أونلاين. |

### setTimeout(double value) {#setTimeout-double-}
```
public final void setTimeout(double value)
```


يضبط المهلة المستخدمة عند انتظار معالجة طلب حفظ المشروع بواسطة خدمة معالجة طابور خادم المشروع. القيمة الافتراضية لهذه الخاصية هي دقيقة واحدة.

--------------------

قد يكون وقت المعالجة أطول للمشروعات الكبيرة أو في حالة عندما يكون مثيل خادم المشروع مشغولًا جدًا في الاستجابة للطلبات الأخرى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double | المهلة المستخدمة عند انتظار معالجة طلب حفظ المشروع بواسطة خدمة معالجة طابور خادم المشروع. |

