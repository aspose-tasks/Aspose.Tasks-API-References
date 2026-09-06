---
title: "ReadOnlyCollectionBase"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Nesnelerin yalnızca okunabilir bir koleksiyonunu temsil eder."
type: docs
weight: 238
url: /tr/java/com.aspose.tasks/readonlycollectionbase/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class ReadOnlyCollectionBase<T> extends AbstractList<T>
```

Nesnelerin yalnızca okunabilir bir koleksiyonunu temsil eder.

T : Koleksiyon öğelerinin türü.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(T item)](#add-T-) | Bu, yalnızca UnsupportedOperationException fırlatan ICollection'ın Add metodunun stub uygulamasıdır. |
| [add(int index, T element)](#add-int-T-) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | Belirtilen indeksteki öğeyi döndürür. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Koleksiyonun yalnızca okunur olup olmadığını belirler. |
| [iterator()](#iterator--) | Bu koleksiyon için bir enumerator döndürür. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [set(int index, T value)](#set-int-T-) | Belirtilen indeksteki öğeyi döndürür. |
| [size()](#size--) | Nesnenin içinde bulunan nesne sayısını alır. |
| [toList()](#toList--) | Koleksiyonu nesne listesine dönüştürür. |
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


Bu, yalnızca UnsupportedOperationException fırlatan ICollection'ın Add metodunun stub uygulamasıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| öğe | T | Eklenecek öğe. |

**Returns:**
boolean
### add(int index, T element) {#add-int-T-}
```
public final void add(int index, T element)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |
| eleman | T | \{@inheritDoc\} |

### clear() {#clear--}
```
public final void clear()
```




### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public final T get(int index)
```


Belirtilen indeksteki öğeyi döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Alınacak öğenin sıfır tabanlı indeksi. |

**Returns:**
T - belirtilen indeksteki eleman.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Koleksiyonun yalnızca okunur olup olmadığını belirler.

**Returns:**
boolean - koleksiyon yalnızca okunur ise true; aksi takdirde false.
### iterator() {#iterator--}
```
public final Iterator<T> iterator()
```


Bu koleksiyon için bir enumerator döndürür.

**Returns:**
java.util.Iterator<T> - Bu koleksiyon için bir yineleyici.
### remove(int index) {#remove-int-}
```
public final T remove(int index)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
T - {@inheritDoc}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### set(int index, T value) {#set-int-T-}
```
public final T set(int index, T value)
```


Belirtilen indeksteki öğeyi döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Alınacak öğenin sıfır tabanlı indeksi. |
| değer | T |  |

**Returns:**
T - belirtilen indeksteki eleman.
### size() {#size--}
```
public final int size()
```


Nesnenin içinde bulunan nesne sayısını alır.

**Returns:**
int - nesnenin içinde bulunan nesne sayısı.
### toList() {#toList--}
```
public final List<T> toList()
```


Koleksiyonu nesne listesine dönüştürür.

**Returns:**
java.util.List<T> - Nesnelerin jenerik listesi.
