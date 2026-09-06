---
title: "OleObjectCollection"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en samling som innehåller instanser av klassen."
type: docs
weight: 165
url: /sv/java/com.aspose.tasks/oleobjectcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public final class OleObjectCollection extends AbstractList<OleObject>
```

Representerar en samling som innehåller instanser av klassen [OleObject](../../com.aspose.tasks/oleobject).
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(OleObject item)](#add-com.aspose.tasks.OleObject-) | \{@inheritDoc\} |
| [clear()](#clear--) | Rensar samlingen. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [size()](#size--) | Returnerar antalet element i denna samling. |
| [toList()](#toList--) | Konverterar instansen av klassen [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) till en lista som innehåller instanser av klassen [OleObject](../../com.aspose.tasks/oleobject). |
### add(OleObject item) {#add-com.aspose.tasks.OleObject-}
```
public boolean add(OleObject item)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | [OleObject](../../com.aspose.tasks/oleobject) | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


Rensar samlingen. För att bevara dessa ändringar bör project.Save anropas med nya MPPSaveOptions \{ WriteViewData = true; \}

--------------------

&gt; ```
&gt; Hur man rensar OLE-objekt och bevarar dessa ändringar.
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
