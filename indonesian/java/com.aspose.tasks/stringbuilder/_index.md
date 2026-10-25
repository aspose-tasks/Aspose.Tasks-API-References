---
title: "StringBuilder"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili string karakter yang dapat diubah."
type: docs
weight: 281
url: /id/java/com.aspose.tasks/stringbuilder/
---

**Inheritance:**
java.lang.Object
```
public final class StringBuilder
```

Mewakili string yang dapat diubah dari karakter. Tidak dapat diperluas.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [StringBuilder()](#StringBuilder--) | Menginisialisasi instance baru dari kelas StringBuilder. |
| [StringBuilder(int capacity)](#StringBuilder-int-) | Menginisialisasi instance baru dari kelas StringBuilder menggunakan kapasitas yang ditentukan. |
| [StringBuilder(int capacity, int maxCapacity)](#StringBuilder-int-int-) | Menginisialisasi instance baru dari kelas StringBuilder yang dimulai dengan kapasitas yang ditentukan dan dapat tumbuh hingga maksimum yang ditentukan. |
| [StringBuilder(String value)](#StringBuilder-java.lang.String-) | Menginisialisasi instance baru dari kelas StringBuilder menggunakan string yang ditentukan. |
| [StringBuilder(String value, int capacity)](#StringBuilder-java.lang.String-int-) | Menginisialisasi instance baru dari kelas StringBuilder menggunakan string dan kapasitas yang ditentukan. |
| [StringBuilder(String value, int startIndex, int length, int capacity)](#StringBuilder-java.lang.String-int-int-int-) | Menginisialisasi instance baru dari kelas StringBuilder dari substring dan kapasitas yang ditentukan. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [append(boolean value)](#append-boolean-) | Menambahkan representasi string dari nilai boolean yang ditentukan ke instance ini. |
| [append(byte value)](#append-byte-) | Menambahkan representasi string dari byte yang ditentukan ke instance ini. |
| [append(char value)](#append-char-) | Menambahkan representasi string dari karakter Unicode yang ditentukan ke instance ini. |
| [append(char value, int repeatCount)](#append-char-int-) | Menambahkan sejumlah salinan yang ditentukan dari representasi string karakter Unicode ke instance ini. |
| [append(char[] value)](#append-char---) | Menambahkan representasi string dari karakter Unicode dalam array yang ditentukan ke instance ini. |
| [append(char[] value, int startIndex, int charCount)](#append-char---int-int-) | Menambahkan representasi string dari subarray karakter Unicode yang ditentukan ke instance ini. |
| [append(double value)](#append-double-) | Menambahkan representasi string dari angka double yang ditentukan ke instance ini. |
| [append(float value)](#append-float-) | Menambahkan representasi string dari angka float yang ditentukan ke instance ini. |
| [append(int value)](#append-int-) | Menambahkan representasi string dari angka int yang ditentukan ke instance ini. |
| [append(Object value)](#append-java.lang.Object-) | Menambahkan representasi string dari objek yang ditentukan ke instance ini. |
| [append(String value)](#append-java.lang.String-) | Menambahkan salinan dari string yang ditentukan ke instance ini. |
| [append(String value, int startIndex, int count)](#append-java.lang.String-int-int-) | Menambahkan salinan dari substring yang ditentukan ke instance ini. |
| [append(BigDecimal value)](#append-java.math.BigDecimal-) | Menambahkan representasi string dari angka BigDecimal yang ditentukan ke instance ini. |
| [append(long value)](#append-long-) | Menambahkan representasi string dari angka long yang ditentukan ke instance ini. |
| [append(short value)](#append-short-) | Menambahkan representasi string dari angka short yang ditentukan ke instance ini. |
| [appendFormat(String format, Object[] args)](#appendFormat-java.lang.String-java.lang.Object...-) | Menambahkan string yang dikembalikan dari pemrosesan string format komposit, yang berisi nol atau lebih item format, ke instance ini. |
| [appendLine()](#appendLine--) | Menambahkan terminator baris default ke akhir objek StringBuilder saat ini. |
| [appendLine(String value)](#appendLine-java.lang.String-) | Menambahkan salinan string yang ditentukan diikuti oleh terminator baris default ke akhir objek StringBuilder saat ini. |
| [copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)](#copyTo-int-char---int-int-) | Menyalin karakter dari segmen tertentu dari instance ini ke segmen tertentu dari array Char tujuan. |
| [ensureCapacity(int capacity)](#ensureCapacity-int-) | Memastikan bahwa kapasitas instance StringBuilder ini setidaknya sebesar nilai yang ditentukan. |
| [equals(Object obj)](#equals-java.lang.Object-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [getCapacity()](#getCapacity--) | Mendapatkan jumlah maksimum karakter yang dapat disimpan dalam memori yang dialokasikan oleh instance saat ini. |
| [getLength()](#getLength--) | Mendapatkan panjang objek StringBuilder saat ini. |
| [getMaxCapacity()](#getMaxCapacity--) | Mendapatkan kapasitas maksimum instance ini. |
| [hashCode()](#hashCode--) | Mengembalikan kode hash untuk StringBuilder ini. |
| [insert(int index, boolean value)](#insert-int-boolean-) | Menyisipkan representasi string dari nilai boolean ke dalam instance ini pada posisi karakter yang ditentukan. |
| [insert(int index, byte value)](#insert-int-byte-) | Menyisipkan representasi string dari nilai byte ke dalam instance ini pada posisi karakter yang ditentukan. |
| [insert(int index, char value)](#insert-int-char-) | Menyisipkan representasi string dari karakter Unicode yang ditentukan ke dalam instance ini pada posisi karakter yang ditentukan. |
| [insert(int index, char[] value)](#insert-int-char---) | Menyisipkan representasi string dari array karakter Unicode yang ditentukan ke dalam instance ini pada posisi karakter yang ditentukan. |
| [insert(int index, char[] value, int startIndex, int charCount)](#insert-int-char---int-int-) | Menyisipkan representasi string dari subarray karakter Unicode yang ditentukan ke dalam instance ini pada posisi karakter yang ditentukan. |
| [insert(int index, double value)](#insert-int-double-) | Menyisipkan representasi string dari angka double ke dalam instance ini pada posisi karakter yang ditentukan. |
| [insert(int index, float value)](#insert-int-float-) | Menyisipkan representasi string dari angka float ke dalam instance ini pada posisi karakter yang ditentukan. |
| [insert(int index, int value)](#insert-int-int-) | Menyisipkan representasi string dari angka int ke dalam instance ini pada posisi karakter yang ditentukan. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | Menyisipkan representasi string dari objek ke dalam instance ini pada posisi karakter yang ditentukan. |
| [insert(int index, String value)](#insert-int-java.lang.String-) | Menyisipkan string ke dalam instance ini pada posisi karakter yang ditentukan. |
| [insert(int index, String value, int count)](#insert-int-java.lang.String-int-) | Menyisipkan satu atau lebih salinan dari string yang ditentukan ke dalam instance ini pada posisi karakter yang ditentukan. |
| [insert(int index, BigDecimal value)](#insert-int-java.math.BigDecimal-) | Menyisipkan representasi string dari angka decimal ke dalam instance ini pada posisi karakter yang ditentukan. |
| [insert(int index, long value)](#insert-int-long-) | Menyisipkan representasi string dari angka long ke dalam instance ini pada posisi karakter yang ditentukan. |
| [insert(int index, short value)](#insert-int-short-) | Menyisipkan representasi string dari angka short ke dalam instance ini pada posisi karakter yang ditentukan. |
| [remove(int startIndex, int length)](#remove-int-int-) | Menghapus rentang karakter yang ditentukan dari instance ini. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Mengganti semua kemunculan karakter yang ditentukan dalam instance ini dengan karakter lain yang ditentukan. |
| [replace(char oldValue, char newValue, int startIndex, int count)](#replace-char-char-int-int-) | Mengganti, dalam sebuah substring dari instance ini, semua kemunculan karakter yang ditentukan dengan karakter lain yang ditentukan. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Mengganti semua kemunculan string yang ditentukan dalam instance ini dengan string lain yang ditentukan. |
| [replace(String oldValue, String newValue, int startIndex, int count)](#replace-java.lang.String-java.lang.String-int-int-) | Mengganti, dalam sebuah substring dari instance ini, semua kemunculan string yang ditentukan dengan string lain yang ditentukan. |
| [setCapacity(int value)](#setCapacity-int-) | Mengatur jumlah maksimum karakter yang dapat disimpan dalam memori yang dialokasikan oleh instance saat ini. |
| [setLength(int value)](#setLength-int-) | Mengatur panjang objek StringBuilder saat ini. |
| [toString()](#toString--) | Mengonversi nilai instance ini menjadi String. |
| [toString(int startIndex, int length)](#toString-int-int-) | Mengonversi nilai substring dari instance ini menjadi String. |
### StringBuilder() {#StringBuilder--}
```
public StringBuilder()
```


Menginisialisasi instance baru dari kelas StringBuilder.

### StringBuilder(int capacity) {#StringBuilder-int-}
```
public StringBuilder(int capacity)
```


Menginisialisasi instance baru dari kelas StringBuilder menggunakan kapasitas yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| kapasitas | int | Ukuran awal yang disarankan untuk instance ini. |

### StringBuilder(int capacity, int maxCapacity) {#StringBuilder-int-int-}
```
public StringBuilder(int capacity, int maxCapacity)
```


Menginisialisasi instance baru dari kelas StringBuilder yang dimulai dengan kapasitas yang ditentukan dan dapat tumbuh hingga maksimum yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| kapasitas | int | Ukuran awal yang disarankan untuk StringBuilder. |
| maxCapacity | int | Jumlah maksimum karakter yang dapat dimuat oleh string saat ini. |

### StringBuilder(String value) {#StringBuilder-java.lang.String-}
```
public StringBuilder(String value)
```


Menginisialisasi instance baru dari kelas StringBuilder menggunakan string yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | String yang digunakan untuk menginisialisasi nilai instance. |

### StringBuilder(String value, int capacity) {#StringBuilder-java.lang.String-int-}
```
public StringBuilder(String value, int capacity)
```


Menginisialisasi instance baru dari kelas StringBuilder menggunakan string dan kapasitas yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | String yang digunakan untuk menginisialisasi nilai instance. |
| kapasitas | int | Ukuran awal yang disarankan untuk StringBuilder. |

### StringBuilder(String value, int startIndex, int length, int capacity) {#StringBuilder-java.lang.String-int-int-int-}
```
public StringBuilder(String value, int startIndex, int length, int capacity)
```


Menginisialisasi instance baru dari kelas StringBuilder dari substring dan kapasitas yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | String yang berisi substring yang digunakan untuk menginisialisasi nilai instance ini. |
| startIndex | int | Posisi dalam nilai di mana substring dimulai. |
| panjang | int | Jumlah karakter dalam substring. |
| kapasitas | int | Ukuran awal yang disarankan untuk StringBuilder. |

### append(boolean value) {#append-boolean-}
```
public StringBuilder append(boolean value)
```


Menambahkan representasi string dari nilai boolean yang ditentukan ke instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | Nilai boolean yang akan ditambahkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(byte value) {#append-byte-}
```
public StringBuilder append(byte value)
```


Menambahkan representasi string dari byte yang ditentukan ke instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | byte | Nilai yang akan ditambahkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value) {#append-char-}
```
public StringBuilder append(char value)
```


Menambahkan representasi string dari karakter Unicode yang ditentukan ke instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | char | Karakter Unicode yang akan ditambahkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char value, int repeatCount) {#append-char-int-}
```
public StringBuilder append(char value, int repeatCount)
```


Menambahkan sejumlah salinan yang ditentukan dari representasi string karakter Unicode ke instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | char | Karakter yang akan ditambahkan. |
| repeatCount | int | Jumlah kali nilai akan ditambahkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value) {#append-char---}
```
public StringBuilder append(char[] value)
```


Menambahkan representasi string dari karakter Unicode dalam array yang ditentukan ke instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | char[] | Array karakter yang akan ditambahkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(char[] value, int startIndex, int charCount) {#append-char---int-int-}
```
public StringBuilder append(char[] value, int startIndex, int charCount)
```


Menambahkan representasi string dari subarray karakter Unicode yang ditentukan ke instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | char[] | Array karakter. |
| startIndex | int | Posisi awal dalam nilai. |
| charCount | int | Jumlah karakter yang akan ditambahkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(double value) {#append-double-}
```
public StringBuilder append(double value)
```


Menambahkan representasi string dari angka double yang ditentukan ke instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | Nilai yang akan ditambahkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(float value) {#append-float-}
```
public StringBuilder append(float value)
```


Menambahkan representasi string dari angka float yang ditentukan ke instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | float | Nilai yang akan ditambahkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(int value) {#append-int-}
```
public StringBuilder append(int value)
```


Menambahkan representasi string dari angka int yang ditentukan ke instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | Nilai yang akan ditambahkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(Object value) {#append-java.lang.Object-}
```
public StringBuilder append(Object value)
```


Menambahkan representasi string dari objek yang ditentukan ke instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.Object | Objek yang akan ditambahkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value) {#append-java.lang.String-}
```
public StringBuilder append(String value)
```


Menambahkan salinan dari string yang ditentukan ke instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | String yang akan ditambahkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(String value, int startIndex, int count) {#append-java.lang.String-int-int-}
```
public StringBuilder append(String value, int startIndex, int count)
```


Menambahkan salinan dari substring yang ditentukan ke instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | String yang berisi substring yang akan ditambahkan. |
| startIndex | int | Posisi awal substring dalam nilai. |
| count | int | Jumlah karakter dalam nilai yang akan ditambahkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(BigDecimal value) {#append-java.math.BigDecimal-}
```
public StringBuilder append(BigDecimal value)
```


Menambahkan representasi string dari angka BigDecimal yang ditentukan ke instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.math.BigDecimal | Nilai yang akan ditambahkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(long value) {#append-long-}
```
public StringBuilder append(long value)
```


Menambahkan representasi string dari angka long yang ditentukan ke instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | long | Nilai yang akan ditambahkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### append(short value) {#append-short-}
```
public StringBuilder append(short value)
```


Menambahkan representasi string dari angka short yang ditentukan ke instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | short | Nilai yang akan ditambahkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendFormat(String format, Object[] args) {#appendFormat-java.lang.String-java.lang.Object...-}
```
public StringBuilder appendFormat(String format, Object[] args)
```


Menambahkan string yang dihasilkan dari memproses string format komposit, yang berisi nol atau lebih item format, ke instance ini. Setiap item format digantikan oleh representasi string dari argumen yang sesuai dalam array parameter.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| format | java.lang.String | String format komposit. |
| args | java.lang.Object[] | Array objek untuk diformat. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with format appended. Each format item in format is replaced by the string representation of the corresponding object argument.
### appendLine() {#appendLine--}
```
public StringBuilder appendLine()
```


Menambahkan terminator baris default ke akhir objek StringBuilder saat ini.

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### appendLine(String value) {#appendLine-java.lang.String-}
```
public StringBuilder appendLine(String value)
```


Menambahkan salinan string yang ditentukan diikuti oleh terminator baris default ke akhir objek StringBuilder saat ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | String yang akan ditambahkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the append operation has completed.
### copyTo(int sourceIndex, char[] destination, int destinationIndex, int count) {#copyTo-int-char---int-int-}
```
public void copyTo(int sourceIndex, char[] destination, int destinationIndex, int count)
```


Menyalin karakter dari segmen tertentu dari instance ini ke segmen tertentu dari array Char tujuan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceIndex | int | Posisi awal dalam instance ini tempat karakter akan disalin. Indeks dimulai dari nol. |
| tujuan | char[] | Array tempat karakter akan disalin. |
| destinationIndex | int | Posisi awal di tujuan tempat karakter akan disalin. Indeksnya berbasis nol. |
| count | int | Jumlah karakter yang akan disalin. |

### ensureCapacity(int capacity) {#ensureCapacity-int-}
```
public int ensureCapacity(int capacity)
```


Memastikan bahwa kapasitas instance StringBuilder ini setidaknya sebesar nilai yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| kapasitas | int | Kapasitas minimum yang harus dipastikan. |

**Returns:**
int - Kapasitas baru dari instance ini.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | java.lang.Object | Objek untuk dibandingkan dengan instance ini, atau null. |

**Returns:**
boolean - true jika instance ini dan sb memiliki nilai string, Capacity, dan MaxCapacity yang sama; jika tidak, false.
### getCapacity() {#getCapacity--}
```
public int getCapacity()
```


Mendapatkan jumlah maksimum karakter yang dapat disimpan dalam memori yang dialokasikan oleh instance saat ini.

**Returns:**
int - Jumlah maksimum karakter yang dapat disimpan dalam memori yang dialokasikan oleh instance saat ini.
### getLength() {#getLength--}
```
public int getLength()
```


Mendapatkan panjang objek StringBuilder saat ini.

**Returns:**
int - Panjang instance ini.
### getMaxCapacity() {#getMaxCapacity--}
```
public int getMaxCapacity()
```


Mendapatkan kapasitas maksimum instance ini.

**Returns:**
int - Jumlah maksimum karakter yang dapat ditampung oleh instance ini.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Mengembalikan kode hash untuk StringBuilder ini.

**Returns:**
int - Mengembalikan nilai kode hash untuk objek ini.
### insert(int index, boolean value) {#insert-int-boolean-}
```
public StringBuilder insert(int index, boolean value)
```


Menyisipkan representasi string dari nilai boolean ke dalam instance ini pada posisi karakter yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Posisi dalam instance ini dimana penyisipan dimulai. |
| nilai | boolean | Nilai yang akan disisipkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, byte value) {#insert-int-byte-}
```
public StringBuilder insert(int index, byte value)
```


Menyisipkan representasi string dari nilai byte ke dalam instance ini pada posisi karakter yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Posisi dalam instance ini dimana penyisipan dimulai. |
| nilai | byte | Nilai yang akan disisipkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char value) {#insert-int-char-}
```
public StringBuilder insert(int index, char value)
```


Menyisipkan representasi string dari karakter Unicode yang ditentukan ke dalam instance ini pada posisi karakter yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Posisi dalam instance ini dimana penyisipan dimulai. |
| nilai | char | Nilai yang akan disisipkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value) {#insert-int-char---}
```
public StringBuilder insert(int index, char[] value)
```


Menyisipkan representasi string dari array karakter Unicode yang ditentukan ke dalam instance ini pada posisi karakter yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Posisi dalam instance ini dimana penyisipan dimulai. |
| nilai | char[] | Array karakter yang akan disisipkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, char[] value, int startIndex, int charCount) {#insert-int-char---int-int-}
```
public StringBuilder insert(int index, char[] value, int startIndex, int charCount)
```


Menyisipkan representasi string dari subarray karakter Unicode yang ditentukan ke dalam instance ini pada posisi karakter yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Posisi dalam instance ini dimana penyisipan dimulai. |
| nilai | char[] | Array karakter. |
| startIndex | int | Indeks awal dalam nilai. |
| charCount | int | Jumlah karakter yang akan disisipkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, double value) {#insert-int-double-}
```
public StringBuilder insert(int index, double value)
```


Menyisipkan representasi string dari angka double ke dalam instance ini pada posisi karakter yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Posisi dalam instance ini dimana penyisipan dimulai. |
| nilai | double | Nilai yang akan disisipkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, float value) {#insert-int-float-}
```
public StringBuilder insert(int index, float value)
```


Menyisipkan representasi string dari angka float ke dalam instance ini pada posisi karakter yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Posisi dalam instance ini dimana penyisipan dimulai. |
| nilai | float | Nilai yang akan disisipkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, int value) {#insert-int-int-}
```
public StringBuilder insert(int index, int value)
```


Menyisipkan representasi string dari angka int ke dalam instance ini pada posisi karakter yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Posisi dalam instance ini dimana penyisipan dimulai. |
| nilai | int | Nilai yang akan disisipkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public StringBuilder insert(int index, Object value)
```


Menyisipkan representasi string dari objek ke dalam instance ini pada posisi karakter yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Posisi dalam instance ini dimana penyisipan dimulai. |
| nilai | java.lang.Object | Objek yang akan disisipkan, atau null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value) {#insert-int-java.lang.String-}
```
public StringBuilder insert(int index, String value)
```


Menyisipkan string ke dalam instance ini pada posisi karakter yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Posisi dalam instance ini dimana penyisipan dimulai. |
| nilai | java.lang.String | String yang akan disisipkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, String value, int count) {#insert-int-java.lang.String-int-}
```
public StringBuilder insert(int index, String value, int count)
```


Menyisipkan satu atau lebih salinan dari string yang ditentukan ke dalam instance ini pada posisi karakter yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Posisi dalam instance ini dimana penyisipan dimulai. |
| nilai | java.lang.String | String yang akan disisipkan. |
| count | int | Jumlah kali nilai akan disisipkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after insertion has completed.
### insert(int index, BigDecimal value) {#insert-int-java.math.BigDecimal-}
```
public StringBuilder insert(int index, BigDecimal value)
```


Menyisipkan representasi string dari angka decimal ke dalam instance ini pada posisi karakter yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Posisi dalam instance ini dimana penyisipan dimulai. |
| nilai | java.math.BigDecimal | Nilai yang akan disisipkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, long value) {#insert-int-long-}
```
public StringBuilder insert(int index, long value)
```


Menyisipkan representasi string dari angka long ke dalam instance ini pada posisi karakter yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Posisi dalam instance ini dimana penyisipan dimulai. |
| nilai | long | Nilai yang akan disisipkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### insert(int index, short value) {#insert-int-short-}
```
public StringBuilder insert(int index, short value)
```


Menyisipkan representasi string dari angka short ke dalam instance ini pada posisi karakter yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | Posisi dalam instance ini dimana penyisipan dimulai. |
| nilai | short | Nilai yang akan disisipkan. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the insert operation has completed.
### remove(int startIndex, int length) {#remove-int-int-}
```
public StringBuilder remove(int startIndex, int length)
```


Menghapus rentang karakter yang ditentukan dari instance ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| startIndex | int | Posisi berbasis nol dalam instance ini dimana penghapusan dimulai. |
| panjang | int | Jumlah karakter yang akan dihapus. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance after the remove operation has completed.
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public StringBuilder replace(char oldChar, char newChar)
```


Mengganti semua kemunculan karakter yang ditentukan dalam instance ini dengan karakter lain yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| oldChar | char | Karakter yang akan diganti. |
| newChar | char | Karakter yang menggantikan oldChar. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar.
### replace(char oldValue, char newValue, int startIndex, int count) {#replace-char-char-int-int-}
```
public StringBuilder replace(char oldValue, char newValue, int startIndex, int count)
```


Mengganti, dalam sebuah substring dari instance ini, semua kemunculan karakter yang ditentukan dengan karakter lain yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| oldValue | char | Karakter yang akan diganti. |
| newValue | char | Karakter yang menggantikan oldChar. |
| startIndex | int | Posisi dalam instance ini di mana substring dimulai. |
| count | int | Panjang substring. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with oldChar replaced by newChar in the range from startIndex to startIndex + count -1.
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public StringBuilder replace(String oldValue, String newValue)
```


Mengganti semua kemunculan string yang ditentukan dalam instance ini dengan string lain yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| oldValue | java.lang.String | String yang akan diganti. |
| newValue | java.lang.String | String yang menggantikan oldValue, atau null. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue.
### replace(String oldValue, String newValue, int startIndex, int count) {#replace-java.lang.String-java.lang.String-int-int-}
```
public StringBuilder replace(String oldValue, String newValue, int startIndex, int count)
```


Mengganti, dalam sebuah substring dari instance ini, semua kemunculan string yang ditentukan dengan string lain yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| oldValue | java.lang.String | String yang akan diganti. |
| newValue | java.lang.String | String yang menggantikan oldValue, atau null. |
| startIndex | int | Posisi dalam instance ini di mana substring dimulai. |
| count | int | Panjang substring. |

**Returns:**
[StringBuilder](../../com.aspose.tasks/stringbuilder) - A reference to this instance with all instances of oldValue replaced by newValue in the range from startIndex to startIndex + count - 1.
### setCapacity(int value) {#setCapacity-int-}
```
public void setCapacity(int value)
```


Mengatur jumlah maksimum karakter yang dapat disimpan dalam memori yang dialokasikan oleh instance saat ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | Jumlah maksimum karakter yang dapat disimpan dalam memori yang dialokasikan oleh instance saat ini. |

### setLength(int value) {#setLength-int-}
```
public void setLength(int value)
```


Mengatur panjang objek StringBuilder saat ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | Panjang instance ini. |

### toString() {#toString--}
```
public String toString()
```


Mengonversi nilai instance ini menjadi String.

**Returns:**
java.lang.String - Sebuah string yang nilainya sama dengan instance ini.
### toString(int startIndex, int length) {#toString-int-int-}
```
public String toString(int startIndex, int length)
```


Mengonversi nilai substring dari instance ini menjadi String.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| startIndex | int | Posisi awal substring dalam instance ini. |
| panjang | int | Panjang substring. |

**Returns:**
java.lang.String - Sebuah string yang nilainya sama dengan substring yang ditentukan dari instance ini.
