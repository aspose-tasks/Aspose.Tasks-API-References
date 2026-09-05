---
title: "OleObjectCollection"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een collectie voor die de instanties van de klasse bevat."
type: docs
weight: 165
url: /nl/java/com.aspose.tasks/oleobjectcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public final class OleObjectCollection extends AbstractList<OleObject>
```

Stelt een collectie voor die de instanties van de [OleObject](../../com.aspose.tasks/oleobject) klasse bevat.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [add(OleObject item)](#add-com.aspose.tasks.OleObject-) | \{@inheritDoc\} |
| [clear()](#clear--) | Leegt de collectie. |
| [get(int index)](#get-int-) | (@inheritDoc\\} |
| [size()](#size--) | Retourneert het aantal elementen in deze collectie. |
| [toList()](#toList--) | Converteert de instantie van de [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) klasse naar een lijst die de instanties van de [OleObject](../../com.aspose.tasks/oleobject) klasse bevat. |
### add(OleObject item) {#add-com.aspose.tasks.OleObject-}
```
public boolean add(OleObject item)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | [OleObject](../../com.aspose.tasks/oleobject) | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


Leegt de collectie. Om deze wijzigingen te behouden moet project.Save worden aangeroepen met new MPPSaveOptions \{ WriteViewData = true; \}

--------------------

&gt; ```
&gt; Hoe OLE-objecten te wissen en deze wijzigingen te behouden.
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
