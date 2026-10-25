---
title: "FilterCriteria"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mendefinisikan kriteria yang harus dipenuhi oleh tugas atau sumber daya agar ditampilkan dalam tampilan MSP."
type: docs
weight: 94
url: /id/java/com.aspose.tasks/filtercriteria/
---

**Inheritance:**
java.lang.Object
```
public class FilterCriteria
```

Mendefinisikan kriteria yang harus dipenuhi oleh tugas atau sumber daya agar ditampilkan dalam tampilan MSP.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [FilterCriteria()](#FilterCriteria--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getCriteriaRows()](#getCriteriaRows--) | Mendapatkan daftar baris anak [FilterCriteria](../../com.aspose.tasks/filtercriteria). |
| [getField()](#getField--) | Mendapatkan sebuah `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) untuk diubah. |
| [getOperation()](#getOperation--) | Mendapatkan kriteria yang ditetapkan dengan FieldName, Test, dan Value yang berhubungan dengan kriteria lain dalam filter. |
| [getTest()](#getTest--) | Mendapatkan tipe perbandingan yang dibuat antara FieldName dan Value yang berfungsi sebagai kriteria seleksi untuk filter. |
| [getValues()](#getValues--) | Mendapatkan nilai objek untuk dibandingkan dengan nilai bidang yang ditentukan dengan FieldName. |
| [isValueAField()](#isValueAField--) | Mendapatkan apakah nilai sisi kanan FilterCriteria adalah referensi bidang, bukan nilai konstan. |
| [isValueAField(int index)](#isValueAField-int-) | Mendapatkan apakah nilai pada indeks FilterCriteria adalah referensi bidang, bukan nilai konstan. |
| [setField(int value)](#setField-int-) | Mengatur sebuah `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) untuk diubah. |
| [setOperation(int value)](#setOperation-int-) | Mengatur kriteria yang ditetapkan dengan FieldName, Test, dan Value yang berhubungan dengan kriteria lain dalam filter. |
| [setTest(int value)](#setTest-int-) | Mengatur tipe perbandingan yang dibuat antara FieldName dan Value yang berfungsi sebagai kriteria seleksi untuk filter. |
| [setValue(int index, Object value)](#setValue-int-java.lang.Object-) | Mengatur nilai objek pada indeks untuk dibandingkan dengan nilai bidang yang ditentukan oleh FieldName. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Mengatur nilai objek untuk dibandingkan dengan nilai bidang yang ditentukan oleh FieldName. |
| [setValueByField(int value)](#setValueByField-int-) | Mengatur bidang yang nilainya akan dibandingkan dengan nilai bidang yang ditentukan oleh FieldName. |
| [setValueByField(int index, int value)](#setValueByField-int-int-) | Mengatur bidang pada indeks yang nilainya akan dibandingkan dengan nilai bidang yang ditentukan oleh FieldName. |
| [toString()](#toString--) | Mengembalikan representasi string dari instance kelas [FilterCriteria](../../com.aspose.tasks/filtercriteria). |
### FilterCriteria() {#FilterCriteria--}
```
public FilterCriteria()
```


### getCriteriaRows() {#getCriteriaRows--}
```
public final List<FilterCriteria> getCriteriaRows()
```


Mendapatkan daftar baris anak [FilterCriteria](../../com.aspose.tasks/filtercriteria). Jika filter berisi lebih dari satu baris kriteria, maka efek dari operator And adalah bahwa kriteria untuk kedua baris harus dipenuhi agar tugas atau sumber daya ditampilkan sebagai hasil filter ini. Efek dari operator Or adalah bahwa kriteria untuk salah satu baris harus dipenuhi.

**Returns:**
java.util.List&lt;com.aspose.tasks.FilterCriteria&gt; - daftar baris anak [FilterCriteria](../../com.aspose.tasks/filtercriteria).
### getField() {#getField--}
```
public final int getField()
```


Mendapatkan sebuah `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) untuk diubah.

**Returns:**
int - sebuah `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) untuk diubah.
### getOperation() {#getOperation--}
```
public final int getOperation()
```


Mendapatkan kriteria yang ditetapkan dengan FieldName, Test, dan Value yang berhubungan dengan kriteria lain dalam filter.

**Returns:**
int - kriteria yang ditetapkan dengan FieldName, Test, dan Value yang berhubungan dengan kriteria lain dalam filter.
### getTest() {#getTest--}
```
public final int getTest()
```


Mendapatkan tipe perbandingan yang dibuat antara FieldName dan Value yang berfungsi sebagai kriteria seleksi untuk filter. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - tipe perbandingan yang dibuat antara FieldName dan Value yang berfungsi sebagai kriteria seleksi untuk filter.
### getValues() {#getValues--}
```
public final Object[] getValues()
```


Mendapatkan nilai objek untuk dibandingkan dengan nilai bidang yang ditentukan dengan FieldName.

**Returns:**
java.lang.Object[] - nilai objek untuk dibandingkan dengan nilai bidang yang ditentukan dengan FieldName.
### isValueAField() {#isValueAField--}
```
public final boolean isValueAField()
```


Mendapatkan apakah nilai sisi kanan FilterCriteria adalah referensi bidang, bukan nilai konstan.

**Returns:**
boolean - apakah nilai sisi kanan FilterCriteria adalah referensi bidang, bukan nilai konstan.
### isValueAField(int index) {#isValueAField-int-}
```
public final boolean isValueAField(int index)
```


Mendapatkan apakah nilai pada indeks FilterCriteria adalah referensi bidang, bukan nilai konstan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | indeks nilai |

**Returns:**
boolean - apakah nilai di sisi kanan pada indeks FilterCriteria adalah referensi bidang, bukan nilai konstan.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Mengatur sebuah `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) untuk diubah.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | int | sebuah `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) untuk diubah. |

### setOperation(int value) {#setOperation-int-}
```
public final void setOperation(int value)
```


Mengatur kriteria yang ditetapkan dengan FieldName, Test, dan Value yang berhubungan dengan kriteria lain dalam filter.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | kriteria yang ditetapkan dengan FieldName, Test, dan Value berhubungan dengan kriteria lain dalam filter. |

### setTest(int value) {#setTest-int-}
```
public final void setTest(int value)
```


Menetapkan tipe perbandingan antara FieldName dan Value yang berfungsi sebagai kriteria seleksi untuk filter. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | tipe perbandingan antara FieldName dan Value yang berfungsi sebagai kriteria seleksi untuk filter. |

### setValue(int index, Object value) {#setValue-int-java.lang.Object-}
```
public final void setValue(int index, Object value)
```


Mengatur nilai objek pada indeks untuk dibandingkan dengan nilai bidang yang ditentukan oleh FieldName.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | indeks nilai. |
| nilai | java.lang.Object | nilai objek yang akan berfungsi sebagai nilai sisi kanan pada indeks kriteria filter. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public final void setValue(Object value)
```


Mengatur nilai objek untuk dibandingkan dengan nilai bidang yang ditentukan oleh FieldName.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.Object | nilai objek yang akan berfungsi sebagai nilai sisi kanan dari kriteria filter. |

### setValueByField(int value) {#setValueByField-int-}
```
public final void setValueByField(int value)
```


Mengatur bidang yang nilainya akan dibandingkan dengan nilai bidang yang ditentukan oleh FieldName.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | Bidang yang akan berfungsi sebagai nilai sisi kanan dari kriteria filter. |

### setValueByField(int index, int value) {#setValueByField-int-int-}
```
public final void setValueByField(int index, int value)
```


Mengatur bidang pada indeks yang nilainya akan dibandingkan dengan nilai bidang yang ditentukan oleh FieldName.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | indeks nilai |
| nilai | int | Bidang yang akan berfungsi sebagai nilai sisi kanan pada indeks kriteria filter. |

### toString() {#toString--}
```
public String toString()
```


Mengembalikan representasi string dari instance kelas [FilterCriteria](../../com.aspose.tasks/filtercriteria).

**Returns:**
java.lang.String - representasi string dari objek ini.
