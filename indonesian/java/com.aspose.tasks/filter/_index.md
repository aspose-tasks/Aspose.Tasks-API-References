---
title: "Filter"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili filter dalam Project."
type: docs
weight: 91
url: /id/java/com.aspose.tasks/filter/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public final class Filter implements Comparable<Filter>, System.IEquatable<Filter>
```

Mewakili filter dalam Project.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Filter()](#Filter--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [compareTo(Filter other)](#compareTo-com.aspose.tasks.Filter-) | Membandingkan instance ini dengan instance yang ditentukan dari kelas [Filter](../../com.aspose.tasks/filter) dan mengembalikan indikasi urutan relatif mereka. |
| [equals(Filter other)](#equals-com.aspose.tasks.Filter-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek AssignmentBaseline yang ditentukan. |
| [equals(Object obj)](#equals-java.lang.Object-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek AssignmentBaseline yang ditentukan. |
| [getCriteria()](#getCriteria--) | Mendapatkan kriteria yang harus dipenuhi oleh tugas atau sumber daya untuk ditampilkan dalam tampilan MSP. |
| [getFilterType()](#getFilterType--) | Mendapatkan tipe filter. |
| [getIndex()](#getIndex--) | Mendapatkan indeks dari objek [Filter](../../com.aspose.tasks/filter) dalam objek yang berisi Filters. |
| [getName()](#getName--) | Mendapatkan nama objek Filter. |
| [getShowInMenu()](#getShowInMenu--) | Menampilkan nilai yang menunjukkan apakah proyek menampilkan nama filter dalam daftar drop-down Filter pada tab View di Ribbon. |
| [getShowRelatedSummaryRows()](#getShowRelatedSummaryRows--) | Mendapatkan nilai yang menunjukkan apakah baris ringkasan terkait ditampilkan untuk filter. |
| [getUid()](#getUid--) | Mendapatkan pengidentifikasi unik dari sebuah filter. |
| [hashCode()](#hashCode--) | Mengembalikan nilai kode hash untuk filter. |
| [op_Equality(Filter a, Filter b)](#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [op_GreaterThan(Filter a, Filter b)](#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Mengembalikan nilai yang menunjukkan apakah instance ini lebih besar dari objek yang ditentukan. |
| [op_GreaterThanOrEqual(Filter a, Filter b)](#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Mengembalikan nilai yang menunjukkan apakah instance ini lebih besar atau sama dengan objek yang ditentukan. |
| [op_Inequality(Filter a, Filter b)](#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Mengembalikan nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan. |
| [op_LessThan(Filter a, Filter b)](#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Mengembalikan nilai yang menunjukkan apakah instance ini lebih kecil dari objek yang ditentukan. |
| [op_LessThanOrEqual(Filter a, Filter b)](#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Mengembalikan nilai yang menunjukkan apakah instance ini lebih kecil atau sama dengan objek yang ditentukan. |
| [setCriteria(FilterCriteria value)](#setCriteria-com.aspose.tasks.FilterCriteria-) | Mengatur kriteria yang harus dipenuhi oleh tugas atau sumber daya agar ditampilkan dalam tampilan MSP. |
| [setFilterType(int value)](#setFilterType-int-) | Tipe filter. |
| [setName(String value)](#setName-java.lang.String-) | Mengatur nama objek Filter. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Mengatur nilai yang menunjukkan apakah proyek menampilkan nama filter dalam daftar drop-down Filter pada tab View di Ribbon. |
| [setShowRelatedSummaryRows(boolean value)](#setShowRelatedSummaryRows-boolean-) | Mengatur nilai yang menunjukkan apakah baris ringkasan terkait ditampilkan untuk filter. |
### Filter() {#Filter--}
```
public Filter()
```


### compareTo(Filter other) {#compareTo-com.aspose.tasks.Filter-}
```
public final int compareTo(Filter other)
```


Membandingkan instance ini dengan instance yang ditentukan dari kelas [Filter](../../com.aspose.tasks/filter) dan mengembalikan indikasi urutan relatif mereka.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | instance yang ditentukan dari kelas [Filter](../../com.aspose.tasks/filter) untuk dibandingkan dengan objek ini. |

**Returns:**
int - indikasi urutan relatif mereka.
### equals(Filter other) {#equals-com.aspose.tasks.Filter-}
```
public final boolean equals(Filter other)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek AssignmentBaseline yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | objek AssignmentBaseline yang ditentukan untuk dibandingkan dengan instance ini. |

**Returns:**
boolean - mengembalikan true jika instance ini sama dengan objek AssignmentBaseline yang ditentukan; jika tidak, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek AssignmentBaseline yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | java.lang.Object | objek AssignmentBaseline yang ditentukan untuk dibandingkan dengan instance ini. |

**Returns:**
boolean - mengembalikan true jika instance ini sama dengan objek AssignmentBaseline yang ditentukan; jika tidak, false.
### getCriteria() {#getCriteria--}
```
public final FilterCriteria getCriteria()
```


Mendapatkan kriteria yang harus dipenuhi oleh tugas atau sumber daya untuk ditampilkan dalam tampilan MSP.

**Returns:**
[FilterCriteria](../../com.aspose.tasks/filtercriteria) - the criteria that tasks or resources must meet to be displayed in MSP view.
### getFilterType() {#getFilterType--}
```
public final int getFilterType()
```


Mendapatkan tipe filter.

**Returns:**
int - tipe filter.
### getIndex() {#getIndex--}
```
public final int getIndex()
```


Mendapatkan indeks dari objek [Filter](../../com.aspose.tasks/filter) dalam objek yang berisi Filters.

**Returns:**
int - indeks dari objek [Filter](../../com.aspose.tasks/filter) dalam objek yang berisi Filters.
### getName() {#getName--}
```
public final String getName()
```


Mendapatkan nama objek Filter.

**Returns:**
java.lang.String - nama objek Filter.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Menampilkan nilai yang menunjukkan apakah proyek menampilkan nama filter dalam daftar drop-down Filter pada tab View di Ribbon.

**Returns:**
boolean - nilai yang menunjukkan apakah proyek menampilkan nama filter di daftar drop-down Filter pada tab View di Ribbon.
### getShowRelatedSummaryRows() {#getShowRelatedSummaryRows--}
```
public final boolean getShowRelatedSummaryRows()
```


Mendapatkan nilai yang menunjukkan apakah baris ringkasan terkait ditampilkan untuk filter.

**Returns:**
boolean - nilai yang menunjukkan apakah baris ringkasan terkait ditampilkan untuk filter.
### getUid() {#getUid--}
```
public final int getUid()
```


Mendapatkan pengidentifikasi unik dari sebuah filter.

**Returns:**
int - pengidentifikasi unik dari sebuah filter.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Mengembalikan nilai kode hash untuk filter.

**Returns:**
int - mengembalikan nilai kode hash untuk objek ini.
### op_Equality(Filter a, Filter b) {#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Equality(Filter a, Filter b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Filter pertama. |
| b | [Filter](../../com.aspose.tasks/filter) | Filter kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan
### op_GreaterThan(Filter a, Filter b) {#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThan(Filter a, Filter b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini lebih besar dari objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Filter pertama. |
| b | [Filter](../../com.aspose.tasks/filter) | Filter kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini lebih besar dari objek yang ditentukan
### op_GreaterThanOrEqual(Filter a, Filter b) {#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThanOrEqual(Filter a, Filter b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini lebih besar atau sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Filter pertama. |
| b | [Filter](../../com.aspose.tasks/filter) | Filter kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini lebih besar dari atau sama dengan objek yang ditentukan
### op_Inequality(Filter a, Filter b) {#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Inequality(Filter a, Filter b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Filter pertama. |
| b | [Filter](../../com.aspose.tasks/filter) | Filter kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan
### op_LessThan(Filter a, Filter b) {#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThan(Filter a, Filter b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini lebih kecil dari objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Filter pertama. |
| b | [Filter](../../com.aspose.tasks/filter) | Filter kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini lebih kecil dari objek yang ditentukan
### op_LessThanOrEqual(Filter a, Filter b) {#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThanOrEqual(Filter a, Filter b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini lebih kecil atau sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | Filter pertama. |
| b | [Filter](../../com.aspose.tasks/filter) | Filter kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini lebih kecil dari atau sama dengan objek yang ditentukan
### setCriteria(FilterCriteria value) {#setCriteria-com.aspose.tasks.FilterCriteria-}
```
public final void setCriteria(FilterCriteria value)
```


Mengatur kriteria yang harus dipenuhi oleh tugas atau sumber daya agar ditampilkan dalam tampilan MSP.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [FilterCriteria](../../com.aspose.tasks/filtercriteria) | kriteria yang harus dipenuhi oleh tugas atau sumber daya agar ditampilkan dalam tampilan MSP. |

### setFilterType(int value) {#setFilterType-int-}
```
public final void setFilterType(int value)
```


Tipe filter.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | tipe filter. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Mengatur nama objek Filter.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nama objek Filter. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Mengatur nilai yang menunjukkan apakah proyek menampilkan nama filter dalam daftar drop-down Filter pada tab View di Ribbon.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah proyek menampilkan nama filter di daftar drop-down Filter pada tab View di Ribbon. |

### setShowRelatedSummaryRows(boolean value) {#setShowRelatedSummaryRows-boolean-}
```
public final void setShowRelatedSummaryRows(boolean value)
```


Mengatur nilai yang menunjukkan apakah baris ringkasan terkait ditampilkan untuk filter.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah baris ringkasan terkait ditampilkan untuk filter. |

