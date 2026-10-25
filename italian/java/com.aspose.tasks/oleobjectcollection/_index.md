---
title: "OleObjectCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una raccolta contenente le istanze della classe."
type: docs
weight: 165
url: /it/java/com.aspose.tasks/oleobjectcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public final class OleObjectCollection extends AbstractList<OleObject>
```

Rappresenta una raccolta contenente le istanze della classe [OleObject](../../com.aspose.tasks/oleobject).
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(OleObject item)](#add-com.aspose.tasks.OleObject-) | \{@inheritDoc\} |
| [clear()](#clear--) | Cancella la raccolta. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [size()](#size--) | Restituisce il numero di elementi in questa raccolta. |
| [toList()](#toList--) | Converte l'istanza della classe [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) in un elenco contenente le istanze della classe [OleObject](../../com.aspose.tasks/oleobject). |
### add(OleObject item) {#add-com.aspose.tasks.OleObject-}
```
public boolean add(OleObject item)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| item | [OleObject](../../com.aspose.tasks/oleobject) | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


Cancella la collezione. Per conservare queste modifiche, project.Save dovrebbe essere chiamato con new MPPSaveOptions \{ WriteViewData = true; \}

--------------------

&gt; ```
&gt; Come cancellare gli oggetti OLE e conservare queste modifiche.
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
