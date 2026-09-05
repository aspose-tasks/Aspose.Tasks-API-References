---
title: "Garis Dasar"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Menampilkan nilai baseline dari sebuah sumber daya."
type: docs
weight: 26
url: /id/java/com.aspose.tasks/baseline/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public class Baseline implements Comparable<Baseline>, System.IEquatable<Baseline>
```

Menampilkan nilai baseline dari sebuah sumber daya.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Baseline()](#Baseline--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [compareTo(Baseline other)](#compareTo-com.aspose.tasks.Baseline-) | Implementasi antarmuka IComparable. |
| [equals(Baseline other)](#equals-com.aspose.tasks.Baseline-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [equals(Object obj)](#equals-java.lang.Object-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [getBaselineNumber()](#getBaselineNumber--) | Mendapatkan nomor unik dari catatan data baseline. |
| [getBcwp()](#getBcwp--) | Mendapatkan biaya yang dianggarkan untuk pekerjaan yang dilakukan oleh sumber daya untuk proyek hingga saat ini. |
| [getBcws()](#getBcws--) | Mendapatkan biaya anggaran untuk pekerjaan yang dijadwalkan bagi sumber daya. |
| [getCost()](#getCost--) | Mendapatkan biaya proyeksi sumber daya ketika baseline disimpan. |
| [getWork()](#getWork--) | Mendapatkan pekerjaan yang ditugaskan kepada sumber daya ketika baseline disimpan. |
| [hashCode()](#hashCode--) | Mengembalikan nilai kode hash untuk baseline. |
| [op_Equality(Baseline a, Baseline b)](#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [op_GreaterThan(Baseline a, Baseline b)](#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Mengembalikan nilai yang menunjukkan apakah instance ini lebih besar dari objek yang ditentukan. |
| [op_GreaterThanOrEqual(Baseline a, Baseline b)](#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Mengembalikan nilai yang menunjukkan apakah instance ini lebih besar atau sama dengan objek yang ditentukan. |
| [op_Inequality(Baseline a, Baseline b)](#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Mengembalikan nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan. |
| [op_LessThan(Baseline a, Baseline b)](#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Mengembalikan nilai yang menunjukkan apakah instance ini lebih kecil dari objek yang ditentukan. |
| [op_LessThanOrEqual(Baseline a, Baseline b)](#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Mengembalikan nilai yang menunjukkan apakah instance ini lebih kecil atau sama dengan objek yang ditentukan. |
| [setBaselineNumber(int value)](#setBaselineNumber-int-) | Mengatur nomor unik untuk catatan data baseline. |
| [setBcwp(double value)](#setBcwp-double-) | Mengatur biaya yang dianggarkan untuk pekerjaan yang dilakukan oleh sumber daya untuk proyek hingga saat ini. |
| [setBcws(double value)](#setBcws-double-) | Mengatur biaya anggaran untuk pekerjaan yang dijadwalkan bagi sumber daya. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Mengatur biaya proyeksi sumber daya ketika baseline disimpan. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Mengatur pekerjaan yang ditugaskan kepada sumber daya ketika baseline disimpan. |
### Baseline() {#Baseline--}
```
public Baseline()
```


### compareTo(Baseline other) {#compareTo-com.aspose.tasks.Baseline-}
```
public final int compareTo(Baseline other)
```


Implementasi antarmuka IComparable. Membandingkan instance ini dengan objek Baseline yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | objek Baseline yang ditentukan untuk dibandingkan dengan instance ini. |

**Returns:**
int - mengembalikan -1 jika instance ini kurang dari objek yang ditentukan, 1 jika instance ini lebih besar dari objek yang ditentukan; jika tidak mengembalikan 0
### equals(Baseline other) {#equals-com.aspose.tasks.Baseline-}
```
public final boolean equals(Baseline other)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | objek yang ditentukan untuk dibandingkan dengan instance ini. |

**Returns:**
boolean - mengembalikan true jika instance ini sama dengan objek yang ditentukan; jika tidak, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | java.lang.Object | objek yang ditentukan untuk dibandingkan dengan instance ini. |

**Returns:**
boolean - mengembalikan true jika instance ini sama dengan objek yang ditentukan; jika tidak, false.
### getBaselineNumber() {#getBaselineNumber--}
```
public final int getBaselineNumber()
```


Mendapatkan nomor unik dari catatan data baseline.

**Returns:**
int - nomor unik untuk catatan data baseline.
### getBcwp() {#getBcwp--}
```
public final double getBcwp()
```


Mendapatkan biaya yang dianggarkan untuk pekerjaan yang dilakukan oleh sumber daya untuk proyek hingga saat ini.

**Returns:**
double - biaya yang dianggarkan untuk pekerjaan yang dilakukan oleh sumber daya untuk proyek hingga saat ini.
### getBcws() {#getBcws--}
```
public final double getBcws()
```


Mendapatkan biaya anggaran untuk pekerjaan yang dijadwalkan bagi sumber daya.

**Returns:**
double - biaya anggaran untuk pekerjaan yang dijadwalkan bagi sumber daya.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Mendapatkan biaya proyeksi sumber daya ketika baseline disimpan.

**Returns:**
java.math.BigDecimal - biaya proyeksi sumber daya ketika baseline disimpan.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Mendapatkan pekerjaan yang ditugaskan kepada sumber daya ketika baseline disimpan.

Value: Jumlah pekerjaan yang ditugaskan kepada sumber daya ketika baseline disimpan.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the work assigned to a resource when the baseline is saved.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Mengembalikan nilai kode hash untuk baseline.

**Returns:**
int - mengembalikan nilai kode hash untuk objek ini.
### op_Equality(Baseline a, Baseline b) {#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Equality(Baseline a, Baseline b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Baseline pertama. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Baseline kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan
### op_GreaterThan(Baseline a, Baseline b) {#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThan(Baseline a, Baseline b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini lebih besar dari objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Baseline pertama. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Baseline kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini lebih besar dari objek yang ditentukan
### op_GreaterThanOrEqual(Baseline a, Baseline b) {#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThanOrEqual(Baseline a, Baseline b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini lebih besar atau sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Baseline pertama. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Baseline kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini lebih besar dari atau sama dengan objek yang ditentukan
### op_Inequality(Baseline a, Baseline b) {#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Inequality(Baseline a, Baseline b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Baseline pertama. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Baseline kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan
### op_LessThan(Baseline a, Baseline b) {#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThan(Baseline a, Baseline b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini lebih kecil dari objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Baseline pertama. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Baseline kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini lebih kecil dari objek yang ditentukan
### op_LessThanOrEqual(Baseline a, Baseline b) {#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThanOrEqual(Baseline a, Baseline b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini lebih kecil atau sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | Baseline pertama. |
| b | [Baseline](../../com.aspose.tasks/baseline) | Baseline kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini lebih kecil dari atau sama dengan objek yang ditentukan
### setBaselineNumber(int value) {#setBaselineNumber-int-}
```
public final void setBaselineNumber(int value)
```


Mengatur nomor unik untuk catatan data baseline.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | nomor unik untuk catatan data baseline. |

### setBcwp(double value) {#setBcwp-double-}
```
public final void setBcwp(double value)
```


Mengatur biaya yang dianggarkan untuk pekerjaan yang dilakukan oleh sumber daya untuk proyek hingga saat ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | biaya yang dianggarkan untuk pekerjaan yang dilakukan oleh sumber daya untuk proyek hingga saat ini. |

### setBcws(double value) {#setBcws-double-}
```
public final void setBcws(double value)
```


Mengatur biaya anggaran untuk pekerjaan yang dijadwalkan bagi sumber daya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | biaya anggaran untuk pekerjaan yang dijadwalkan bagi sumber daya. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Mengatur biaya proyeksi sumber daya ketika baseline disimpan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.math.BigDecimal | biaya proyeksi sumber daya ketika baseline disimpan. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Mengatur pekerjaan yang ditugaskan kepada sumber daya ketika baseline disimpan.

Value: Jumlah pekerjaan yang ditugaskan kepada sumber daya ketika baseline disimpan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | pekerjaan yang ditugaskan kepada sumber daya ketika baseline disimpan. |

