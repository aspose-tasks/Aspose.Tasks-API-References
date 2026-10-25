---
title: "RateCollection"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili koleksi yang berisi objek."
type: docs
weight: 234
url: /id/java/com.aspose.tasks/ratecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractMap

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RateCollection extends AbstractMap<Integer,RateByDateCollection> implements Iterable<Map.Entry<Integer,RateByDateCollection>>
```

Mewakili koleksi yang berisi objek [Rate](../../com.aspose.tasks/rate).
## Metode

| Metode | Deskripsi |
| --- | --- |
| [add(Date ratesFrom)](#add-java.util.Date-) | Menambahkan sebuah instance [Rate](../../com.aspose.tasks/rate) baru ke koleksi ini. |
| [add(Date ratesFrom, int type)](#add-java.util.Date-int-) | Menambahkan sebuah instance [Rate](../../com.aspose.tasks/rate) baru ke koleksi ini. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [entrySet()](#entrySet--) | (@inheritDoc\} |
| [get(Object key)](#get-java.lang.Object-) | (@inheritDoc\} |
| [getByRateType(int key)](#getByRateType-int-) | Mengembalikan elemen pada indeks yang ditentukan. |
| [getParentResource()](#getParentResource--) | Mendapatkan objek [Resource](../../com.aspose.tasks/resource) induk untuk koleksi ini. |
| [isReadOnly()](#isReadOnly--) | Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca. |
| [iterator()](#iterator--) | Mengembalikan enumerator untuk koleksi ini. |
| [put(Integer key, RateByDateCollection value)](#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-) | (@inheritDoc\} |
| [remove(Rate item)](#remove-com.aspose.tasks.Rate-) | Menghapus instance Rate dari koleksi ini. |
| [setByRateType(int key, RateByDateCollection value)](#setByRateType-int-com.aspose.tasks.RateByDateCollection-) | Menetapkan elemen pada indeks yang ditentukan. |
| [size()](#size--) | Mendapatkan jumlah elemen yang terdapat dalam RateCollection. |
| [toList()](#toList--) | Mengonversi objek [RateCollection](../../com.aspose.tasks/ratecollection) menjadi daftar objek [Rate](../../com.aspose.tasks/rate). |
| [toList(int type)](#toList-int-) | Mengonversi objek [RateCollection](../../com.aspose.tasks/ratecollection) menjadi daftar objek [Rate](../../com.aspose.tasks/rate) yang difilter berdasarkan tipe [RateType](../../com.aspose.tasks/ratetype) yang ditentukan. |
### add(Date ratesFrom) {#add-java.util.Date-}
```
public final Rate add(Date ratesFrom)
```


Menambahkan sebuah instance [Rate](../../com.aspose.tasks/rate) baru ke koleksi ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| ratesFrom | java.util.Date | Tanggal ketika tarif baru mulai berlaku. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### add(Date ratesFrom, int type) {#add-java.util.Date-int-}
```
public final Rate add(Date ratesFrom, int type)
```


Menambahkan sebuah instance [Rate](../../com.aspose.tasks/rate) baru ke koleksi ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| ratesFrom | java.util.Date | Tanggal ketika tarif baru mulai berlaku. |
| type | int | Tabel tarif yang akan ditambahkan. |

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
java.util.Set&lt;java.util.Map.Entry&lt;java.lang.Integer,com.aspose.tasks.RateByDateCollection&gt;&gt; - \\{@inheritDoc\\}
### get(Object key) {#get-java.lang.Object-}
```
public final RateByDateCollection get(Object key)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### getByRateType(int key) {#getByRateType-int-}
```
public final RateByDateCollection getByRateType(int key)
```


Mengembalikan elemen pada indeks yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| key | int | Indeks berbasis nol dari elemen yang akan diambil. |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - the element at the specified index.
### getParentResource() {#getParentResource--}
```
public final Resource getParentResource()
```


Mendapatkan objek [Resource](../../com.aspose.tasks/resource) induk untuk koleksi ini.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - the parent [Resource](../../com.aspose.tasks/resource) object for this collection.
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca.

**Returns:**
boolean - nilai yang menunjukkan apakah koleksi ini hanya-baca.
### iterator() {#iterator--}
```
public final Iterator iterator()
```


Mengembalikan enumerator untuk koleksi ini.

**Returns:**
java.util.Iterator - enumerator untuk koleksi ini.
### put(Integer key, RateByDateCollection value) {#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-}
```
public final RateByDateCollection put(Integer key, RateByDateCollection value)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| key | java.lang.Integer | \{@inheritDoc\} |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### remove(Rate item) {#remove-com.aspose.tasks.Rate-}
```
public final boolean remove(Rate item)
```


Menghapus instance Rate dari koleksi ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | [Rate](../../com.aspose.tasks/rate) | Item yang akan dihapus. |

**Returns:**
boolean - true jika Rate yang ditentukan berhasil dihapus; jika tidak, false.
### setByRateType(int key, RateByDateCollection value) {#setByRateType-int-com.aspose.tasks.RateByDateCollection-}
```
public final void setByRateType(int key, RateByDateCollection value)
```


Menetapkan elemen pada indeks yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| key | int | Indeks berbasis nol dari elemen yang akan diatur. |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | Elemen yang akan diatur pada indeks yang ditentukan. |

### size() {#size--}
```
public final int size()
```


Mendapatkan jumlah elemen yang terdapat dalam RateCollection.

**Returns:**
int - jumlah elemen yang terdapat dalam RateCollection.
### toList() {#toList--}
```
public final List<Rate> toList()
```


Mengonversi objek [RateCollection](../../com.aspose.tasks/ratecollection) menjadi daftar objek [Rate](../../com.aspose.tasks/rate).

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - Daftar objek [Rate](../../com.aspose.tasks/rate).
### toList(int type) {#toList-int-}
```
public final List<Rate> toList(int type)
```


Mengonversi objek [RateCollection](../../com.aspose.tasks/ratecollection) menjadi daftar objek [Rate](../../com.aspose.tasks/rate) yang difilter berdasarkan tipe [RateType](../../com.aspose.tasks/ratetype) yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| type | int | Tipe yang akan difilter. |

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - sebuah daftar objek [Rate](../../com.aspose.tasks/rate).
