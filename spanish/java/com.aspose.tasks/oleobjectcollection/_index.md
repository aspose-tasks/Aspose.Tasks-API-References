---
title: "OleObjectCollection"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una colección que contiene las instancias de la clase."
type: docs
weight: 165
url: /es/java/com.aspose.tasks/oleobjectcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public final class OleObjectCollection extends AbstractList<OleObject>
```

Representa una colección que contiene las instancias de la clase [OleObject](../../com.aspose/tasks/oleobject).
## Métodos

| Método | Descripción |
| --- | --- |
| [add(OleObject item)](#add-com.aspose.tasks.OleObject-) | \{@inheritDoc\} |
| [clear()](#clear--) | Borra la colección. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [size()](#size--) | Devuelve el número de elementos en esta colección. |
| [toList()](#toList--) | Convierte la instancia de la clase [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) a una lista que contiene las instancias de la clase [OleObject](../../com.aspose.tasks/oleobject). |
### add(OleObject item) {#add-com.aspose.tasks.OleObject-}
```
public boolean add(OleObject item)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| item | [OleObject](../../com.aspose.tasks/oleobject) | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


Borra la colección. Para conservar estos cambios, se debe llamar a project.Save con new MPPSaveOptions \{ WriteViewData = true; \}

--------------------

&gt; ```
&gt; Cómo borrar objetos OLE y conservar estos cambios.
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
