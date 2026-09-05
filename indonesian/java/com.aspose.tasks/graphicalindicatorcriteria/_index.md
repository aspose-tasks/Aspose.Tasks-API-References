---
title: "GraphicalIndicatorCriteria"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili satu kriteria indikator grafis yang terkait dengan atribut tambahan."
type: docs
weight: 115
url: /id/java/com.aspose.tasks/graphicalindicatorcriteria/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteria
```

Mewakili satu kriteria indikator grafis yang terkait dengan atribut tambahan.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Menginisialisasi instance baru dari tipe [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria). |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Menginisialisasi instance baru dari tipe [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getImageIndex()](#getImageIndex--) | Mendapatkan indeks gambar yang akan ditampilkan ketika bidang memenuhi kriteria. |
| [getRowType()](#getRowType--) | Mendapatkan nilai enum [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) yang menunjukkan untuk baris mana indikator diterapkan. |
| [getTest()](#getTest--) | Mendapatkan jenis perbandingan yang dibuat antara nilai atribut yang diperluas dan Nilai yang berfungsi sebagai kriteria untuk penerapan indikator grafis. |
| [getValue1()](#getValue1--) | Mendapatkan nilai yang digunakan untuk menguji nilai atribut yang diperluas. |
| [getValue2()](#getValue2--) | Mendapatkan nilai kedua yang digunakan untuk menguji nilai atribut yang diperluas dalam kasus tipe perbandingan 'IsWithin' dan 'IsNotWithin'. |
| [toString()](#toString--) | Mengembalikan representasi string dari instance kelas [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria). |
### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)
```


Menginisialisasi instance baru dari tipe [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| rowType | int | nilai enum [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) yang menunjukkan untuk baris mana indikator diterapkan |
| test | int | nilai [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) yang menunjukkan jenis perbandingan yang dilakukan oleh kriteria. |
| imageIndex | int | indeks gambar yang akan ditampilkan ketika bidang memenuhi kriteria |
| value1 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | nilai yang digunakan dalam pemeriksaan kondisi. |
| value2 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | nilai kedua (akhir interval) yang digunakan dalam pemeriksaan kondisi dalam kasus kondisi 'IsWithin' dan 'IsNotWithing'. |

### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```


Menginisialisasi instance baru dari tipe [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| rowType | int | nilai enum [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) yang menunjukkan untuk baris mana indikator diterapkan |
| test | int | nilai [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) yang menunjukkan jenis perbandingan yang dilakukan oleh kriteria. |
| imageIndex | int | indeks gambar yang akan ditampilkan ketika bidang memenuhi kriteria |
| value | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | nilai yang digunakan dalam pemeriksaan kondisi. |

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Mendapatkan indeks gambar yang akan ditampilkan ketika bidang memenuhi kriteria.

**Returns:**
int - indeks gambar yang akan ditampilkan ketika bidang memenuhi kriteria.
### getRowType() {#getRowType--}
```
public final int getRowType()
```


Mendapatkan nilai enum [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) yang menunjukkan untuk baris mana indikator diterapkan.

**Returns:**
int - nilai enum [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) yang menunjukkan untuk baris mana indikator diterapkan.
### getTest() {#getTest--}
```
public final int getTest()
```


Mendapatkan jenis perbandingan yang dibuat antara nilai atribut yang diperluas dan Nilai yang berfungsi sebagai kriteria untuk penerapan indikator grafis. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - jenis perbandingan yang dibuat antara nilai atribut yang diperluas dan Nilai yang berfungsi sebagai kriteria untuk penerapan indikator grafis.
### getValue1() {#getValue1--}
```
public final GraphicalIndicatorCriteriaValue getValue1()
```


Mendapatkan nilai yang digunakan untuk menguji nilai atribut yang diperluas.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the value used to test extended attribute's value.
### getValue2() {#getValue2--}
```
public final GraphicalIndicatorCriteriaValue getValue2()
```


Mendapatkan nilai kedua yang digunakan untuk menguji nilai atribut yang diperluas dalam kasus tipe perbandingan 'IsWithin' dan 'IsNotWithin'.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the second value used to test extended attribute's value in case of 'IsWithin' and 'IsNotWithin' comparison types.
### toString() {#toString--}
```
public String toString()
```


Mengembalikan representasi string dari instance kelas [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria).

**Returns:**
java.lang.String - representasi string dari objek ini.
