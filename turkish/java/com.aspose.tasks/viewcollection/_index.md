---
title: "ViewCollection"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Nesnelerin bir listesini içerir."
type: docs
weight: 343
url: /tr/java/com.aspose.tasks/viewcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class ViewCollection extends AbstractCollection<View>
```

[View](../../com.aspose.tasks/view) nesnelerinin bir listesini içerir. `AbstractCollection` sınıfını genişletir.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(View item)](#add-com.aspose.tasks.View-) | Belirtilen öğeyi bu koleksiyona ekler. |
| [clear()](#clear--) | Bu koleksiyondaki tüm öğeleri kaldırır. |
| [contains(View item)](#contains-com.aspose.tasks.View-) | Belirtilen öğe bu koleksiyonda bulunursa true döndürür; aksi takdirde false. |
| [copyTo(View[] array, int arrayIndex)](#copyTo-com.aspose.tasks.View---int-) | Bu koleksiyonun öğelerini belirtilen diziye, belirtilen dizi indeksinden başlayarak kopyalar. |
| [getByName(String viewName)](#getByName-java.lang.String-) | İsme sahip bir View arar ve koleksiyon içinde ilk oluşumu döndürür. |
| [getByViewScreen(int screen)](#getByViewScreen-int-) | Belirtilen Screen özelliğine sahip bir View arar ve koleksiyon içinde ilk oluşumu döndürür. |
| [getParentProject()](#getParentProject--) | View nesnesinin üst nesnesini alır. |
| [iterator()](#iterator--) | Bu koleksiyonda bulunan öğeler üzerinde bir yineleyici döndürür. |
| [remove(View item)](#remove-com.aspose.tasks.View-) | Bu koleksiyondan belirli bir nesnenin ilk oluşumunu kaldırır. |
| [size()](#size--) | Bu koleksiyonda bulunan öğe sayısını alır. |
| [toList()](#toList--) | Bir view koleksiyonunu [View](../../com.aspose.tasks/view) nesnelerinin listesine dönüştürür. |
### add(View item) {#add-com.aspose.tasks.View-}
```
public final boolean add(View item)
```


Belirtilen öğeyi bu koleksiyona ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | Bu koleksiyona eklenecek belirtilen öğe. |

**Returns:**
boolean - işlem başarılıysa true.
### clear() {#clear--}
```
public final void clear()
```


Bu koleksiyondaki tüm öğeleri kaldırır.

### contains(View item) {#contains-com.aspose.tasks.View-}
```
public final boolean contains(View item)
```


Belirtilen öğe bu koleksiyonda bulunursa true döndürür; aksi takdirde false.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | bulunacak belirtilen öğe. |

**Returns:**
boolean - belirtilen öğe bu koleksiyonda bulunursa true; aksi takdirde false.
### copyTo(View[] array, int arrayIndex) {#copyTo-com.aspose.tasks.View---int-}
```
public final void copyTo(View[] array, int arrayIndex)
```


Bu koleksiyonun öğelerini belirtilen diziye, belirtilen dizi indeksinden başlayarak kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| array | [View\[\]](../../com.aspose.tasks/view) | öğeleri kopyalamak için belirtilen tek boyutlu dizi |
| arrayIndex | int | kopyalamanın başladığı belirtilen dizinin sıfır tabanlı indeksi. |

### getByName(String viewName) {#getByName-java.lang.String-}
```
public final View getByName(String viewName)
```


İsme sahip bir View arar ve koleksiyon içinde ilk oluşumu döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| viewName | java.lang.String | Aranacak View'un adı. |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection with the specified name, if found; otherwise, null.
### getByViewScreen(int screen) {#getByViewScreen-int-}
```
public final View getByViewScreen(int screen)
```


Belirtilen Screen özelliğine sahip bir View arar ve koleksiyon içinde ilk oluşumu döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| screen | int | [ViewScreen](../../com.aspose.tasks/viewscreen) enum değer. |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection which Screen property matches the specified screen argument, if found; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


View nesnesinin üst öğesini alır. Salt okunur [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### iterator() {#iterator--}
```
public Iterator<View> iterator()
```


Bu koleksiyonda bulunan öğeler üzerinde bir yineleyici döndürür.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.View&gt; - koleksiyon yineleyicisi.
### remove(View item) {#remove-com.aspose.tasks.View-}
```
public final boolean remove(View item)
```


Bu koleksiyondan belirli bir nesnenin ilk oluşumunu kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | kaldırılacak belirtilen nesne. |

**Returns:**
boolean - belirtilen nesne bu koleksiyondan başarıyla kaldırıldıysa true; aksi takdirde false.
### size() {#size--}
```
public final int size()
```


Bu koleksiyonda bulunan öğe sayısını alır.

**Returns:**
int - bu koleksiyonda bulunan öğe sayısı.
### toList() {#toList--}
```
public final List<View> toList()
```


Bir view koleksiyonunu [View](../../com.aspose.tasks/view) nesnelerinin listesine dönüştürür.

**Returns:**
java.util.List&lt;com.aspose.tasks.View&gt; - [View](../../com.aspose.tasks/view) nesnelerinin genel listesi.
