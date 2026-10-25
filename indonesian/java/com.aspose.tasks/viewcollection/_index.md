---
title: "ViewCollection"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Berisi daftar objek."
type: docs
weight: 343
url: /id/java/com.aspose.tasks/viewcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class ViewCollection extends AbstractCollection<View>
```

Berisi daftar objek [View](../../com.aspose.tasks/view). Memperluas kelas `AbstractCollection`.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [add(View item)](#add-com.aspose.tasks.View-) | Menambahkan item yang ditentukan ke koleksi ini. |
| [clear()](#clear--) | Menghapus semua item dari koleksi ini. |
| [contains(View item)](#contains-com.aspose.tasks.View-) | Mengembalikan true jika item yang ditentukan ditemukan dalam koleksi ini; jika tidak, false. |
| [copyTo(View[] array, int arrayIndex)](#copyTo-com.aspose.tasks.View---int-) | Menyalin elemen-elemen koleksi ini ke array yang ditentukan, mulai dari indeks array yang ditentukan. |
| [getByName(String viewName)](#getByName-java.lang.String-) | Mencari View dengan nama tersebut, dan mengembalikan kemunculan pertama dalam koleksi. |
| [getByViewScreen(int screen)](#getByViewScreen-int-) | Mencari View dengan properti Screen yang ditentukan, dan mengembalikan kemunculan pertama dalam koleksi. |
| [getParentProject()](#getParentProject--) | Mengambil induk dari objek View. |
| [iterator()](#iterator--) | Mengembalikan iterator atas elemen yang terdapat dalam koleksi ini. |
| [remove(View item)](#remove-com.aspose.tasks.View-) | Menghapus kemunculan pertama dari objek tertentu dalam koleksi ini. |
| [size()](#size--) | Mendapatkan jumlah elemen yang terdapat dalam koleksi ini. |
| [toList()](#toList--) | Mengonversi koleksi view menjadi daftar objek [View](../../com.aspose.tasks/view). |
### add(View item) {#add-com.aspose.tasks.View-}
```
public final boolean add(View item)
```


Menambahkan item yang ditentukan ke koleksi ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | item yang ditentukan untuk ditambahkan ke koleksi ini. |

**Returns:**
boolean - true jika operasi berhasil.
### clear() {#clear--}
```
public final void clear()
```


Menghapus semua item dari koleksi ini.

### contains(View item) {#contains-com.aspose.tasks.View-}
```
public final boolean contains(View item)
```


Mengembalikan true jika item yang ditentukan ditemukan dalam koleksi ini; jika tidak, false.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | item yang ditentukan untuk dicari. |

**Returns:**
boolean - true jika item yang ditentukan ditemukan dalam koleksi ini; jika tidak, false.
### copyTo(View[] array, int arrayIndex) {#copyTo-com.aspose.tasks.View---int-}
```
public final void copyTo(View[] array, int arrayIndex)
```


Menyalin elemen-elemen koleksi ini ke array yang ditentukan, mulai dari indeks array yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| array | [View\[\]](../../com.aspose.tasks/view) | array satu dimensi yang ditentukan untuk menyalin elemen ke |
| arrayIndex | int | indeks berbasis nol dari array yang ditentukan di mana penyalinan dimulai. |

### getByName(String viewName) {#getByName-java.lang.String-}
```
public final View getByName(String viewName)
```


Mencari View dengan nama tersebut, dan mengembalikan kemunculan pertama dalam koleksi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| viewName | java.lang.String | Nama View yang akan dicari. |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection with the specified name, if found; otherwise, null.
### getByViewScreen(int screen) {#getByViewScreen-int-}
```
public final View getByViewScreen(int screen)
```


Mencari View dengan properti Screen yang ditentukan, dan mengembalikan kemunculan pertama dalam koleksi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| screen | int | nilai enumerasi [ViewScreen](../../com.aspose.tasks/viewscreen). |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection which Screen property matches the specified screen argument, if found; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Mendapatkan induk dari objek View. Hanya-baca [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### iterator() {#iterator--}
```
public Iterator<View> iterator()
```


Mengembalikan iterator atas elemen yang terdapat dalam koleksi ini.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.View&gt; - iterator koleksi.
### remove(View item) {#remove-com.aspose.tasks.View-}
```
public final boolean remove(View item)
```


Menghapus kemunculan pertama dari objek tertentu dalam koleksi ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | objek yang ditentukan untuk dihapus. |

**Returns:**
boolean - true jika objek yang ditentukan berhasil dihapus dari koleksi ini; jika tidak, false.
### size() {#size--}
```
public final int size()
```


Mendapatkan jumlah elemen yang terdapat dalam koleksi ini.

**Returns:**
int - jumlah elemen yang terdapat dalam koleksi ini.
### toList() {#toList--}
```
public final List<View> toList()
```


Mengonversi koleksi view menjadi daftar objek [View](../../com.aspose.tasks/view).

**Returns:**
java.util.List&lt;com.aspose.tasks.View&gt; - Daftar generik dari objek [View](../../com.aspose.tasks/view).
