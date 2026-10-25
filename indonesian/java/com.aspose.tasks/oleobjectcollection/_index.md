---
title: "OleObjectCollection"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili koleksi yang berisi instance dari kelas tersebut."
type: docs
weight: 165
url: /id/java/com.aspose.tasks/oleobjectcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public final class OleObjectCollection extends AbstractList<OleObject>
```

Mewakili koleksi yang berisi instance dari kelas [OleObject](../../com.aspose.tasks/oleobject).
## Metode

| Metode | Deskripsi |
| --- | --- |
| [add(OleObject item)](#add-com.aspose.tasks.OleObject-) | \{@inheritDoc\} |
| [clear()](#clear--) | Menghapus koleksi. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [size()](#size--) | Mengembalikan jumlah elemen dalam koleksi ini. |
| [toList()](#toList--) | Mengonversi instance dari kelas [OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) menjadi daftar yang berisi instance dari kelas [OleObject](../../com.aspose.tasks/oleobject). |
### add(OleObject item) {#add-com.aspose.tasks.OleObject-}
```
public boolean add(OleObject item)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | [OleObject](../../com.aspose.tasks/oleobject) | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


Menghapus koleksi. Untuk mempertahankan perubahan ini project.Save harus dipanggil dengan MPPSaveOptions baru \{ WriteViewData = true; \}

--------------------

&gt; ```
&gt; Cara menghapus objek OLE dan mempertahankan perubahan ini.
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
