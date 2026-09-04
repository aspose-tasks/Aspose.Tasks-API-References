---
title: "ResourceViewColumn"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "فئة عرض المشاريع المستخدمة في عرض ResourceUsage وعرض ResourceSheet."
type: docs
weight: 261
url: /ar/java/com.aspose.tasks/resourceviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class ResourceViewColumn extends ViewColumn
```

فئة عرض المشروع المستخدمة في عرض ResourceUsage وعرض ResourceSheet.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-) | ينشئ مثيلاً جديداً من الفئة [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-) | ينشئ مثيلاً جديداً من الفئة [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
| [ResourceViewColumn(int width, int field)](#ResourceViewColumn-int-int-) | ينشئ مثيلاً جديداً من الفئة [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getColumnText(Resource resource)](#getColumnText-com.aspose.tasks.Resource-) | يحوّل المورد الحالي إلى نص العمود. |
| [getField()](#getField--) | يعيد حقل العمود. |
| [setField(int value)](#setField-int-) | يضبط حقل العمود. |
### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)
```


ينشئ مثيلاً جديداً من الفئة [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم العمود. |
| width | int | عرض العمود بالبكسل. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | محول بيانات المورد إلى نص العمود. |
| حقل | int | حقل العمود. |

### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)
```


ينشئ مثيلاً جديداً من الفئة [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم العمود. |
| width | int | عرض العمود بالبكسل. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | محول بيانات المورد إلى نص العمود. |

### ResourceViewColumn(int width, int field) {#ResourceViewColumn-int-int-}
```
public ResourceViewColumn(int width, int field)
```


ينشئ مثيلاً جديداً من الفئة [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| width | int | عرض العمود بالبكسل. |
| حقل | int | حقل العمود. |

### getColumnText(Resource resource) {#getColumnText-com.aspose.tasks.Resource-}
```
public final String getColumnText(Resource resource)
```


يحوّل المورد الحالي إلى نص العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| resource | [Resource](../../com.aspose.tasks/resource) | المورد الحالي. |

**Returns:**
java.lang.String - نص العمود.
### getField() {#getField--}
```
public int getField()
```


يعيد حقل العمود. `Field`.

**Returns:**
int - قيمة حقل العمود.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


يضبط حقل العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | قيمة حقل العمود. |

