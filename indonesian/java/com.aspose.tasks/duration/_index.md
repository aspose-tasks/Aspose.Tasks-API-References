---
title: "Duration"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili durasi dalam sebuah proyek."
type: docs
weight: 76
url: /id/java/com.aspose.tasks/duration/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public class Duration extends Struct<Duration> implements System.IEquatable<Duration>
```

Mewakili durasi dalam sebuah proyek.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Duration()](#Duration--) | Menginisialisasi instance baru dari struct [Duration](../../com.aspose.tasks/duration) dengan nilai TimeSpan dan TimeUnitType yang ditentukan. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [Clone()](#Clone--) | Membuat dan mengembalikan salinan mendalam dari instance ini. |
| [CloneTo(Duration that)](#CloneTo-com.aspose.tasks.Duration-) | Membuat salinan mendalam dari instance ke instance lain. |
| [add(Duration d)](#add-com.aspose.tasks.Duration-) | Menambahkan durasi yang ditentukan ke durasi ini. |
| [add(double val)](#add-double-) | Menambahkan nilai double yang ditentukan ke durasi ini. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [convert(byte timeUnitType)](#convert-byte-) | Mengonversi objek Duration ke durasi lain dengan satuan waktu yang ditentukan. |
| [equals(Duration other)](#equals-com.aspose.tasks.Duration-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [equals(Duration obj1, Duration obj2)](#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Mengembalikan nilai yang menunjukkan apakah instance `obj1` yang ditentukan sama dengan instance `obj2` yang ditentukan. |
| [equals(Object obj)](#equals-java.lang.Object-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [getTimeSpan()](#getTimeSpan--) | Mendapatkan instance `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) dari objek Duration ini. |
| [getTimeUnit()](#getTimeUnit--) | Mendapatkan tipe unit waktu untuk objek ini. |
| [hashCode()](#hashCode--) | Mengembalikan nilai kode hash untuk objek ini. |
| [isElapsed()](#isElapsed--) | Mendapatkan nilai yang menunjukkan apakah unit waktu telah berlalu. |
| [isEstimated()](#isEstimated--) | Mendapatkan nilai yang menunjukkan apakah unit waktu diperkirakan. |
| [op_Equality(Duration a, Duration b)](#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [op_Inequality(Duration a, Duration b)](#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Mengembalikan nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan. |
| [parse(Project p, String value)](#parse-com.aspose.tasks.Project-java.lang.String-) | Mengonversi string yang ditentukan menjadi instance dari struktur [Duration](../../com.aspose.tasks/duration). |
| [parseTimeSpan(String value)](#parseTimeSpan-java.lang.String-) | Menganalisis string durasi dalam format "PT--H--M--S--". |
| [subtract(Duration d)](#subtract-com.aspose.tasks.Duration-) | Mengurangi durasi yang ditentukan dari instance durasi ini. |
| [subtract(double val)](#subtract-double-) | Mengurangi nilai double yang ditentukan dari instance durasi ini. |
| [toDouble()](#toDouble--) | Mengonversi objek Duration menjadi nilai `double`. |
| [toString()](#toString--) | Mengembalikan representasi string dari instance ini. |
### Duration() {#Duration--}
```
public Duration()
```


Menginisialisasi instance baru dari struct [Duration](../../com.aspose.tasks/duration) dengan nilai TimeSpan dan TimeUnitType yang ditentukan.

### Clone() {#Clone--}
```
public Duration Clone()
```


Membuat dan mengembalikan salinan mendalam dari instance ini.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a deep copy of this object.
### CloneTo(Duration that) {#CloneTo-com.aspose.tasks.Duration-}
```
public void CloneTo(Duration that)
```


Membuat salinan mendalam dari instance ke instance lain.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| that | [Duration](../../com.aspose.tasks/duration) | instansi lain. |

### add(Duration d) {#add-com.aspose.tasks.Duration-}
```
public final Duration add(Duration d)
```


Menambahkan durasi yang ditentukan ke durasi ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | [Duration](../../com.aspose.tasks/duration) yang ditentukan untuk ditambahkan ke instance ini. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### add(double val) {#add-double-}
```
public final Duration add(double val)
```


Menambahkan nilai double yang ditentukan ke durasi ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| val | double | `double` yang ditentukan untuk ditambahkan ke instance ini. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### convert(byte timeUnitType) {#convert-byte-}
```
public final Duration convert(byte timeUnitType)
```


Mengonversi objek Duration ke durasi lain dengan satuan waktu yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| timeUnitType | byte | tipe unit waktu yang ditentukan. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - returns new duration with the specified unit type.
### equals(Duration other) {#equals-com.aspose.tasks.Duration-}
```
public final boolean equals(Duration other)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | [Duration](../../com.aspose.tasks/duration) | Objek untuk dibandingkan dengan instance ini. |

**Returns:**
boolean - Mengembalikan **True** jika instance Duration lain memiliki nilai TimeSpan dan TimeUnit yang sama dengan instance ini; jika tidak, **false**.
### equals(Duration obj1, Duration obj2) {#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean equals(Duration obj1, Duration obj2)
```


Mengembalikan nilai yang menunjukkan apakah instance `obj1` yang ditentukan sama dengan instance `obj2` yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj1 | [Duration](../../com.aspose.tasks/duration) | objek pertama untuk dibandingkan. |
| obj2 | [Duration](../../com.aspose.tasks/duration) | objek kedua untuk dibandingkan. |

**Returns:**
boolean - mengembalikan true jika instansi `obj1` yang ditentukan sama dengan instansi `obj2` yang ditentukan; jika tidak, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | java.lang.Object | Objek untuk dibandingkan dengan instance ini. |

**Returns:**
boolean - **True** jika objek yang ditentukan adalah Duration yang memiliki nilai TimeSpan dan TimeUnit yang sama dengan instance ini; jika tidak, **false**.
### getTimeSpan() {#getTimeSpan--}
```
public final double getTimeSpan()
```


Mendapatkan instance `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) dari objek Duration ini.

Nilai: Instance TimeSpan dari objek Duration ini.

**Returns:**
double - instance `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) dari objek Duration ini.
### getTimeUnit() {#getTimeUnit--}
```
public final byte getTimeUnit()
```


Mendapatkan tipe unit waktu untuk objek ini.

Nilai: Tipe unit waktu dari instance Duration ini.

**Returns:**
byte - tipe unit waktu untuk objek ini.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Mengembalikan nilai kode hash untuk objek ini.

**Returns:**
int - mengembalikan nilai kode hash untuk instance durasi ini.
### isElapsed() {#isElapsed--}
```
public final boolean isElapsed()
```


Mendapatkan nilai yang menunjukkan apakah unit waktu telah berlalu.

Nilai: Bendera yang menentukan apakah instance Duration ini telah berlalu.

**Returns:**
boolean - nilai yang menunjukkan apakah unit waktu telah berlalu.
### isEstimated() {#isEstimated--}
```
public final boolean isEstimated()
```


Mendapatkan nilai yang menunjukkan apakah unit waktu diperkirakan.

Nilai: Bendera yang menentukan apakah instance Duration ini diperkirakan.

**Returns:**
boolean - nilai yang menunjukkan apakah unit waktu diperkirakan.
### op_Equality(Duration a, Duration b) {#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Equality(Duration a, Duration b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | Durasi pertama. |
| b | [Duration](../../com.aspose.tasks/duration) | Durasi kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan
### op_Inequality(Duration a, Duration b) {#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Inequality(Duration a, Duration b)
```


Mengembalikan nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | Durasi pertama. |
| b | [Duration](../../com.aspose.tasks/duration) | Durasi kedua. |

**Returns:**
boolean - nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan
### parse(Project p, String value) {#parse-com.aspose.tasks.Project-java.lang.String-}
```
public static Duration parse(Project p, String value)
```


Mengonversi string yang ditentukan menjadi instance dari struktur [Duration](../../com.aspose.tasks/duration).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| p | [Project](../../com.aspose.tasks/project) | instansi yang ditentukan dari kelas [Project](../../com.aspose.tasks/project) untuk mengonversi durasi. |
| nilai | java.lang.String | string yang ditentukan untuk dikonversi. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Returns the converted instance of [Duration](../../com.aspose.tasks/duration) struct.
### parseTimeSpan(String value) {#parseTimeSpan-java.lang.String-}
```
public static double parseTimeSpan(String value)
```


Menganalisis string durasi dalam format "PT--H--M--S--".

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | string yang ditentukan untuk diparsing. |

**Returns:**
double - mengembalikan instansi yang diparsing dari struct `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)).
### subtract(Duration d) {#subtract-com.aspose.tasks.Duration-}
```
public final Duration subtract(Duration d)
```


Mengurangi durasi yang ditentukan dari instance durasi ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | instansi [Duration](../../com.aspose.tasks/duration) yang ditentukan untuk dikurangkan dari instansi ini. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### subtract(double val) {#subtract-double-}
```
public final Duration subtract(double val)
```


Mengurangi nilai double yang ditentukan dari instance durasi ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| val | double | nilai `double` yang ditentukan untuk dikurangkan dari instansi ini. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### toDouble() {#toDouble--}
```
public final double toDouble()
```


Mengonversi objek Duration menjadi nilai `double`.

**Returns:**
double - Nilai yang dikonversi.
### toString() {#toString--}
```
public String toString()
```


Mengembalikan representasi string dari instance ini.

**Returns:**
java.lang.String - representasi string dari instansi ini.
