---
title: "DbSettings"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يسمح بتحديد الإعدادات للقراءة من قاعدة بيانات المشروع."
type: docs
weight: 75
url: /ar/java/com.aspose.tasks/dbsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class DbSettings
```

يسمح بتحديد الإعدادات للقراءة من قاعدة بيانات المشروع.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getConnectionString()](#getConnectionString--) | يحصل على سلسلة الاتصال. |
| [getDriverClassName()](#getDriverClassName--) | يرجع اسم فئة برنامج تشغيل JDBC. |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | يضبط سلسلة الاتصال. |
| [setDriverClassName(String value)](#setDriverClassName-java.lang.String-) | يضبط اسم فئة برنامج تشغيل JDBC. |
### getConnectionString() {#getConnectionString--}
```
public final String getConnectionString()
```


يحصل على سلسلة الاتصال.

**Returns:**
java.lang.String - سلسلة الاتصال.
### getDriverClassName() {#getDriverClassName--}
```
public final String getDriverClassName()
```


يرجع اسم فئة برنامج تشغيل JDBC. اسم فئة البرنامج الافتراضي هو "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Returns:**
java.lang.String - سلسلة فئة البرنامج.
### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public final void setConnectionString(String value)
```


يضبط سلسلة الاتصال.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | سلسلة الاتصال. |

### setDriverClassName(String value) {#setDriverClassName-java.lang.String-}
```
public final void setDriverClassName(String value)
```


يضبط اسم فئة برنامج تشغيل JDBC. اسم فئة البرنامج الافتراضي هو "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | اسم فئة برنامج تشغيل JDBC. |

