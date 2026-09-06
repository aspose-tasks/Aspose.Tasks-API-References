---
title: "OleObjectCollection"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Belirtilen sınıfın örneklerini içeren bir koleksiyonu temsil eder."
type: docs
weight: 165
url: /tr/java/com.aspose.tasks/oleobjectcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public final class OleObjectCollection extends AbstractList<OleObject>
```

Belirtilen [OleObject](../../com.aspose.tasks/oleobject) sınıfının örneklerini içeren bir koleksiyonu temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(OleObject item)](#add-com.aspose.tasks.OleObject-) | \{@inheritDoc\} |
| [clear()](#clear--) | Koleksiyonu temizler. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [size()](#size--) | Bu koleksiyondaki öğe sayısını döndürür. |
| [toList()](#toList--) | [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) sınıfının örneğini, [OleObject](../../com.aspose.tasks/oleobject) sınıfının örneklerini içeren bir listeye dönüştürür. |
### add(OleObject item) {#add-com.aspose.tasks.OleObject-}
```
public boolean add(OleObject item)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| item | [OleObject](../../com.aspose.tasks/oleobject) | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


Koleksiyonu temizler. Bu değişiklikleri kalıcı hâle getirmek için project.Save, yeni MPPSaveOptions \{ WriteViewData = true; \} ile çağrılmalıdır.

--------------------

&gt; ```
&gt; OLE nesnelerini nasıl temizler ve bu değişiklikleri nasıl kalıcı hâle getirirsin.
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
