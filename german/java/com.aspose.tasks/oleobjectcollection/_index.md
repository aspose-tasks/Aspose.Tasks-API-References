---
title: "OleObjectCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Sammlung dar, die die Instanzen der  Klasse enthält."
type: docs
weight: 165
url: /de/java/com.aspose.tasks/oleobjectcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public final class OleObjectCollection extends AbstractList<OleObject>
```

Stellt eine Sammlung dar, die die Instanzen der [OleObject](../../com.aspose/tasks/oleobject) Klasse enthält.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(OleObject item)](#add-com.aspose.tasks.OleObject-) | \{@inheritDoc\} |
| [clear()](#clear--) | Leert die Sammlung. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [size()](#size--) | Gibt die Anzahl der Elemente in dieser Sammlung zurück. |
| [toList()](#toList--) | Konvertiert die Instanz der [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) Klasse in eine Liste, die die Instanzen der [OleObject](../../com.aspose.tasks/oleobject) Klasse enthält. |
### add(OleObject item) {#add-com.aspose.tasks.OleObject-}
```
public boolean add(OleObject item)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | [OleObject](../../com.aspose.tasks/oleobject) | \{@inheritDoc\} |

**Returns:**
boolean - \\{@inheritDoc\\}
### clear() {#clear--}
```
public final void clear()
```


Leert die Sammlung. Um diese Änderungen zu speichern, sollte project.Save mit neuen MPPSaveOptions \\{ WriteViewData = true; \\} aufgerufen werden.

--------------------

&gt; ```
&gt; Wie man OLE-Objekte löscht und diese Änderungen speichert.
&gt; ``````

 [C#]
project.OleObjects.Clear();
project.Save(\"output.mpp\", new MPPSaveOptions {WriteViewData = true;} )
 
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
