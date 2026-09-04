---
title: "OleObjectCollection"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل مجموعة تحتوي على مثيلات الفئة."
type: docs
weight: 165
url: /ar/java/com.aspose.tasks/oleobjectcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public final class OleObjectCollection extends AbstractList<OleObject>
```

يمثل مجموعة تحتوي على مثيلات الفئة [OleObject](../../com.aspose.tasks/oleobject).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(OleObject item)](#add-com.aspose.tasks.OleObject-) | \{@inheritDoc\} |
| [clear()](#clear--) | يمسح المجموعة. |
| [get(int index)](#get-int-) | (@inheritDoc\\} |
| [size()](#size--) | يعيد عدد العناصر في هذه المجموعة. |
| [toList()](#toList--) | يحوّل مثيل الفئة [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) إلى قائمة تحتوي على مثيلات الفئة [OleObject](../../com.aspose.tasks/oleobject). |
### add(OleObject item) {#add-com.aspose.tasks.OleObject-}
```
public boolean add(OleObject item)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| item | [OleObject](../../com.aspose.tasks/oleobject) | \{@inheritDoc\} |

**Returns:**
منطقي - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


يمسح المجموعة. من أجل حفظ هذه التغييرات يجب استدعاء project.Save مع MPPSaveOptions جديد \{ WriteViewData = true; \}

--------------------

&gt; ```
&gt; كيفية مسح كائنات OLE وحفظ هذه التغييرات.
&gt; ``````

 [C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
 
```



### get(int index) {#get-int-}
```
public OleObject get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[OleObject](../../com.aspose.tasks/oleobject) - \{@inheritDoc\}
### size() {#size--}
```
public int size()
```


Returns the number of elements in this collection.

**Returns:**
int - the number of elements in this collection.
### toList() {#toList--}
```
public final List<OleObject> toList()
```


Converts the instance of the [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) class to a list containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class.

**Returns:**
java.util.List&lt;com.aspose.tasks.OleObject&gt; - Converted to list the instance of the [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) class containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class.
