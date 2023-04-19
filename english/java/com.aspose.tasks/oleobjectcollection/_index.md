---
title: OleObjectCollection
second_title: Aspose.Tasks for Java API Reference
description: Represents a collection containing the instances of the  class.
type: docs
weight: 154
url: /java/com.aspose.tasks/oleobjectcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public final class OleObjectCollection extends AbstractList<OleObject>
```

Represents a collection containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class.
## Methods

| Method | Description |
| --- | --- |
| [add(OleObject item)](#add-com.aspose.tasks.OleObject-) | \{@inheritDoc\} |
| [clear()](#clear--) | Clears the collection. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [size()](#size--) | Returns the number of elements in this collection. |
| [toList()](#toList--) | Converts the instance of the [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) class to a list containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class. |
### add(OleObject item) {#add-com.aspose.tasks.OleObject-}
```
public boolean add(OleObject item)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [OleObject](../../com.aspose.tasks/oleobject) | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


Clears the collection. In order to persist these changes project.Save should be called with new MPPSaveOptions \{ WriteViewData = true; \}

--------------------

&gt; ```
&gt; How to clear OLE objects and persist these changes.
&gt;  ```
&gt; 
&gt;  [C#]
&gt;  project.OleObjects.Clear();
&gt;  project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
&gt;  
&gt; ```
&gt; ```

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
