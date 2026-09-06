---
title: "RateCollection"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Nesneleri içeren bir koleksiyonu temsil eder."
type: docs
weight: 234
url: /tr/java/com.aspose.tasks/ratecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractMap

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RateCollection extends AbstractMap<Integer,RateByDateCollection> implements Iterable<Map.Entry<Integer,RateByDateCollection>>
```

Nesneleri içeren bir koleksiyonu temsil eder [Rate](../../com.aspose.tasks/rate) nesnelerini.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(Date ratesFrom)](#add-java.util.Date-) | Bu koleksiyona yeni bir [Rate](../../com.aspose.tasks/rate) örneği ekler. |
| [add(Date ratesFrom, int type)](#add-java.util.Date-int-) | Bu koleksiyona yeni bir [Rate](../../com.aspose.tasks/rate) örneği ekler. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [entrySet()](#entrySet--) | (@inheritDoc\} |
| [get(Object key)](#get-java.lang.Object-) | (@inheritDoc\} |
| [getByRateType(int key)](#getByRateType-int-) | Belirtilen indeksteki öğeyi döndürür. |
| [getParentResource()](#getParentResource--) | Bu koleksiyon için üst [Resource](../../com.aspose.tasks/resource) nesnesini alır. |
| [isReadOnly()](#isReadOnly--) | Bu koleksiyonun yalnızca okunabilir olup olmadığını gösteren bir değeri alır. |
| [iterator()](#iterator--) | Bu koleksiyon için bir enumerator döndürür. |
| [put(Integer key, RateByDateCollection value)](#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-) | (@inheritDoc\} |
| [remove(Rate item)](#remove-com.aspose.tasks.Rate-) | Bu koleksiyondan Rate örneğini kaldırır. |
| [setByRateType(int key, RateByDateCollection value)](#setByRateType-int-com.aspose.tasks.RateByDateCollection-) | Belirtilen indeksteki öğeyi ayarlar. |
| [size()](#size--) | RateCollection içinde bulunan öğe sayısını alır. |
| [toList()](#toList--) | [RateCollection](../../com.aspose.tasks/ratecollection) nesnesini [Rate](../../com.aspose.tasks/rate) nesnelerinin bir listesine dönüştürür. |
| [toList(int type)](#toList-int-) | [RateCollection](../../com.aspose.tasks/ratecollection) nesnesini belirtilen [RateType](../../com.aspose.tasks/ratetype) türüne göre filtrelenmiş [Rate](../../com.aspose.tasks/rate) nesnelerinin bir listesine dönüştürür. |
### add(Date ratesFrom) {#add-java.util.Date-}
```
public final Rate add(Date ratesFrom)
```


Bu koleksiyona yeni bir [Rate](../../com.aspose.tasks/rate) örneği ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ratesFrom | java.util.Date | Yeni oranın yürürlüğe girdiği tarih. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### add(Date ratesFrom, int type) {#add-java.util.Date-int-}
```
public final Rate add(Date ratesFrom, int type)
```


Bu koleksiyona yeni bir [Rate](../../com.aspose.tasks/rate) örneği ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ratesFrom | java.util.Date | Yeni oranın yürürlüğe girdiği tarih. |
| tür | int | Eklenecek oran tablosu. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### clear() {#clear--}
```
public final void clear()
```




### entrySet() {#entrySet--}
```
public Set<Map.Entry<Integer,RateByDateCollection>> entrySet()
```


(@inheritDoc\}

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;java.lang.Integer,com.aspose.tasks.RateByDateCollection&gt;&gt; - \{@inheritDoc\}
### get(Object key) {#get-java.lang.Object-}
```
public final RateByDateCollection get(Object key)
```


(@inheritDoc\}

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| anahtar | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### getByRateType(int key) {#getByRateType-int-}
```
public final RateByDateCollection getByRateType(int key)
```


Belirtilen indeksteki öğeyi döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| anahtar | int | Alınacak öğenin sıfır tabanlı indeksi. |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - the element at the specified index.
### getParentResource() {#getParentResource--}
```
public final Resource getParentResource()
```


Bu koleksiyon için üst [Resource](../../com.aspose.tasks/resource) nesnesini alır.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - the parent [Resource](../../com.aspose.tasks/resource) object for this collection.
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Bu koleksiyonun yalnızca okunabilir olup olmadığını gösteren bir değeri alır.

**Returns:**
boolean - bu koleksiyonun yalnızca okunabilir olup olmadığını gösteren bir değer.
### iterator() {#iterator--}
```
public final Iterator iterator()
```


Bu koleksiyon için bir enumerator döndürür.

**Returns:**
java.util.Iterator - bu koleksiyon için bir yineleyici.
### put(Integer key, RateByDateCollection value) {#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-}
```
public final RateByDateCollection put(Integer key, RateByDateCollection value)
```


(@inheritDoc\}

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| anahtar | java.lang.Integer | \{@inheritDoc\} |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### remove(Rate item) {#remove-com.aspose.tasks.Rate-}
```
public final boolean remove(Rate item)
```


Bu koleksiyondan Rate örneğini kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| item | [Rate](../../com.aspose.tasks/rate) | Kaldırılacak öğe. |

**Returns:**
boolean - belirtilen Rate başarıyla kaldırıldıysa true; aksi takdirde false.
### setByRateType(int key, RateByDateCollection value) {#setByRateType-int-com.aspose.tasks.RateByDateCollection-}
```
public final void setByRateType(int key, RateByDateCollection value)
```


Belirtilen indeksteki öğeyi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| anahtar | int | Ayarlanacak öğenin sıfır tabanlı indeksi. |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | Belirtilen indekste ayarlanacak öğe. |

### size() {#size--}
```
public final int size()
```


RateCollection içinde bulunan öğe sayısını alır.

**Returns:**
int - RateCollection içinde bulunan öğe sayısı.
### toList() {#toList--}
```
public final List<Rate> toList()
```


[RateCollection](../../com.aspose.tasks/ratecollection) nesnesini [Rate](../../com.aspose.tasks/rate) nesnelerinin bir listesine dönüştürür.

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - [Rate](../../com.aspose.tasks/rate) nesnelerinin listesi.
### toList(int type) {#toList-int-}
```
public final List<Rate> toList(int type)
```


[RateCollection](../../com.aspose.tasks/ratecollection) nesnesini belirtilen [RateType](../../com.aspose.tasks/ratetype) türüne göre filtrelenmiş [Rate](../../com.aspose.tasks/rate) nesnelerinin bir listesine dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tür | int | Filtrelenecek tip. |

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - [Rate](../../com.aspose.tasks/rate) nesnelerinin bir listesi.
