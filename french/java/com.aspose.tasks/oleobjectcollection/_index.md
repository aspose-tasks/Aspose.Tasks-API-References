---
title: "OleObjectCollection"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une collection contenant les instances de la classe."
type: docs
weight: 165
url: /fr/java/com.aspose.tasks/oleobjectcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public final class OleObjectCollection extends AbstractList<OleObject>
```

Représente une collection contenant les instances de la classe [OleObject](../../com.aspose/tasks/oleobject).
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(OleObject item)](#add-com.aspose.tasks.OleObject-) | \{@inheritDoc\} |
| [clear()](#clear--) | Efface la collection. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [size()](#size--) | Renvoie le nombre d'éléments dans cette collection. |
| [toList()](#toList--) | Convertit l'instance de la classe [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) en une liste contenant les instances de la classe [OleObject](../../com.aspose.tasks/oleobject). |
### add(OleObject item) {#add-com.aspose.tasks.OleObject-}
```
public boolean add(OleObject item)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| item | [OleObject](../../com.aspose.tasks/oleobject) | \{@inheritDoc\} |

**Returns:**
booléen - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


Efface la collection. Afin de persister ces modifications, project.Save doit être appelé avec new MPPSaveOptions \{ WriteViewData = true; \}

--------------------

&gt; ```
&gt; Comment effacer les objets OLE et persister ces modifications.
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
