---
title: "PropertyKeyedCollection"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Kelas dasar dari kumpulan properti."
type: docs
weight: 231
url: /id/java/com.aspose.tasks/propertykeyedcollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection

**All Implemented Interfaces:**
java.util.Collection
```
public abstract class PropertyKeyedCollection<T> extends PropertyCollection<T> implements Collection<T>
```

Kelas dasar dari kumpulan properti.

T : tipe properti.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [&lt;T1&gt;toArray(T1[] a)](#-T1-toArray-T1---) | \{@inheritDoc\} |
| [add(T item)](#add-T-) | Membuat properti khusus baru. |
| [addAll(Collection&lt;? extends T&gt; c)](#addAll-java.util.Collection---extends-T--) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object item)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [contains(String name)](#contains-java.lang.String-) | Menentukan apakah Aspose.Tasks.Properties.PropertyCollection<T> berisi properti dengan nama yang ditentukan. |
| [containsAll(Collection&lt;?&gt; c)](#containsAll-java.util.Collection----) | \{@inheritDoc\} |
| [getNames()](#getNames--) | Mendapatkan koleksi semua nama properti. |
| [get_Item(String name)](#get-Item-java.lang.String-) | Mendapatkan Property yang terkait dengan kunci yang ditentukan. |
| [isEmpty()](#isEmpty--) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca; jika tidak, false. |
| [remove(Object item)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [removeAll(Collection&lt;?&gt; c)](#removeAll-java.util.Collection----) | \{@inheritDoc\} |
| [retainAll(Collection&lt;?&gt; c)](#retainAll-java.util.Collection----) | \{@inheritDoc\} |
| [size()](#size--) | Mendapatkan jumlah properti dalam koleksi. |
| [toArray()](#toArray--) | \{@inheritDoc\} |
### &lt;T1&gt;toArray(T1[] a) {#-T1-toArray-T1---}
```
public T1[] <T1>toArray(T1[] a)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | T1[] | \{@inheritDoc\} |

**Returns:**
T1[] - {@inheritDoc}
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


Membuat properti khusus baru.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | T | Properti yang akan ditambahkan. |

**Returns:**
boolean
### addAll(Collection&lt;? extends T&gt; c) {#addAll-java.util.Collection---extends-T--}
```
public boolean addAll(Collection<? extends T> c)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| c | java.util.Collection<? extends T> | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public void clear()
```




### contains(Object item) {#contains-java.lang.Object-}
```
public final boolean contains(Object item)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | java.lang.Object |  |

**Returns:**
boolean
### contains(String name) {#contains-java.lang.String-}
```
public final boolean contains(String name)
```


Menentukan apakah Aspose.Tasks.Properties.PropertyCollection<T> berisi properti dengan nama yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | java.lang.String | Nama sebuah properti |

**Returns:**
boolean - true jika Aspose.Tasks.Properties.PropertyCollection<T> berisi properti dengan nama yang ditentukan; jika tidak, false.
### containsAll(Collection&lt;?&gt; c) {#containsAll-java.util.Collection----}
```
public boolean containsAll(Collection<?> c)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### getNames() {#getNames--}
```
public final Collection<String> getNames()
```


Mendapatkan koleksi semua nama properti.

**Returns:**
java.util.Collection<java.lang.String> - koleksi semua nama properti.
### get_Item(String name) {#get-Item-java.lang.String-}
```
public final T get_Item(String name)
```


Mendapatkan Property yang terkait dengan kunci yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | java.lang.String | Nama Property yang akan diambil. |

**Returns:**
T - Property yang terkait dengan nama yang ditentukan.
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```




**Returns:**
boolean - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca; jika tidak, false.

**Returns:**
boolean - nilai yang menunjukkan apakah koleksi ini hanya-baca; jika tidak, false.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### removeAll(Collection&lt;?&gt; c) {#removeAll-java.util.Collection----}
```
public boolean removeAll(Collection<?> c)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### retainAll(Collection&lt;?&gt; c) {#retainAll-java.util.Collection----}
```
public boolean retainAll(Collection<?> c)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| c | java.util.Collection<?> | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


Mendapatkan jumlah properti dalam koleksi.

**Returns:**
int - jumlah properti dalam koleksi.
### toArray() {#toArray--}
```
public Object[] toArray()
```




**Returns:**
java.lang.Object[] - {@inheritDoc}
