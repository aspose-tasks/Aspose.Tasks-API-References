---
title: "FilterCollection"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Nesnelerin bir listesini içerir."
type: docs
weight: 92
url: /tr/java/com.aspose.tasks/filtercollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class FilterCollection extends AbstractCollection<Filter>
```

Bir [Filter](../../com.aspose.tasks/filter) nesnesi listesi içerir. ICollection&lt;Filter&gt; arayüzünü uygular.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(Filter item)](#add-com.aspose.tasks.Filter-) |  |
| [clear()](#clear--) | Bu koleksiyondaki tüm öğeleri kaldırır (isteğe bağlı işlem). |
| [contains(Filter item)](#contains-com.aspose.tasks.Filter-) | Bu koleksiyon belirtilen öğeyi içeriyorsa true döndürür. |
| [copyTo(Filter[] array, int arrayIndex)](#copyTo-com.aspose.tasks.Filter---int-) | Belirtilen diziden öğeleri, belirtilen indeksten başlayarak bu koleksiyona kopyalar. |
| [iterator()](#iterator--) | Bu koleksiyonda bulunan öğeler üzerinde bir yineleyici döndürür. |
| [remove(Filter item)](#remove-com.aspose.tasks.Filter-) | Belirtilen öğeyi bu koleksiyondan kaldırır. |
| [size()](#size--) | Bu koleksiyonda bulunan öğe sayısını alır. |
| [toList()](#toList--) | Bir filtre koleksiyonunu `Filter` nesnelerinin bir listesine dönüştürür. |
### add(Filter item) {#add-com.aspose.tasks.Filter-}
```
public boolean add(Filter item)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) |  |

**Returns:**
boolean
### clear() {#clear--}
```
public void clear()
```


Bu koleksiyondaki tüm öğeleri kaldırır (isteğe bağlı işlem).

### contains(Filter item) {#contains-com.aspose.tasks.Filter-}
```
public final boolean contains(Filter item)
```


Bu koleksiyon belirtilen öğeyi içeriyorsa true döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | belirtilen öğe. |

**Returns:**
boolean - koleksiyon belirtilen öğeyi içeriyorsa true.
### copyTo(Filter[] array, int arrayIndex) {#copyTo-com.aspose.tasks.Filter---int-}
```
public final void copyTo(Filter[] array, int arrayIndex)
```


Belirtilen diziden öğeleri, belirtilen indeksten başlayarak bu koleksiyona kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| array | [Filter\[\]](../../com.aspose.tasks/filter) | öğeleri kopyalamak için belirtilen tek boyutlu dizi |
| arrayIndex | int | kopyalamanın başladığı belirtilen dizinin sıfır tabanlı indeksi. |

### iterator() {#iterator--}
```
public Iterator<Filter> iterator()
```


Bu koleksiyonda bulunan öğeler üzerinde bir yineleyici döndürür.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Filter&gt; - koleksiyon yineleyicisi.
### remove(Filter item) {#remove-com.aspose.tasks.Filter-}
```
public final boolean remove(Filter item)
```


Belirtilen öğeyi bu koleksiyondan kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | belirtilen öğe. |

**Returns:**
boolean - işlem başarılıysa true.
### size() {#size--}
```
public final int size()
```


Bu koleksiyonda bulunan öğe sayısını alır.

**Returns:**
int - bu koleksiyonda bulunan öğe sayısı.
### toList() {#toList--}
```
public List<Filter> toList()
```


Bir filtre koleksiyonunu `Filter` nesnelerinin bir listesine dönüştürür.

**Returns:**
java.util.List&lt;com.aspose.tasks.Filter&gt; - `Filter` nesnelerinin genel listesi.
