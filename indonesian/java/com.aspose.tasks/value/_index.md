---
title: "Nilai"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili nilai dalam daftar nilai."
type: docs
weight: 333
url: /id/java/com.aspose.tasks/value/
---

**Inheritance:**
java.lang.Object
```
public class Value
```

Mewakili nilai dalam daftar nilai.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Value()](#Value--) | Menginisialisasi instance baru dari kelas [Value](../../com.aspose/tasks/value). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getDateValue()](#getDateValue--) | Mendapatkan nilai aktual jika dapat direpresentasikan sebagai DateTime. |
| [getDescription()](#getDescription--) | Mendapatkan deskripsi dari sebuah nilai. |
| [getDuration()](#getDuration--) | Mendapatkan nilai aktual yang digunakan untuk merepresentasikan Durasi. |
| [getId()](#getId--) | Mendapatkan pengidentifikasi unik dari sebuah nilai di seluruh proyek. |
| [getNumericValue()](#getNumericValue--) | Mendapatkan nilai aktual yang digunakan untuk merepresentasikan nilai angka atau biaya. |
| [getPhonetic()](#getPhonetic--) | Mendapatkan informasi fonetik tentang nama bidang khusus. |
| [getStringValue()](#getStringValue--) | Mendapatkan nilai aktual yang digunakan untuk merepresentasikan string Teks. |
| [getVal()](#getVal--) | Mendapatkan nilai aktual dalam representasi internal. |
| [getValueGuid()](#getValueGuid--) | Mendapatkan GUID yang mengidentifikasi nilai ini di antara yang lain dalam seluruh proyek. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Mengatur nilai aktual jika dapat direpresentasikan sebagai DateTime. |
| [setDescription(String value)](#setDescription-java.lang.String-) | Mengatur deskripsi dari sebuah nilai. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Mengatur nilai aktual yang digunakan untuk merepresentasikan Durasi. |
| [setId(int value)](#setId-int-) | Mengatur pengidentifikasi unik dari sebuah nilai di seluruh proyek. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Mengatur nilai aktual yang digunakan untuk merepresentasikan nilai angka atau biaya. |
| [setPhonetic(String value)](#setPhonetic-java.lang.String-) | Mengatur informasi fonetik tentang nama bidang khusus. |
| [setStringValue(String value)](#setStringValue-java.lang.String-) | Mengatur nilai aktual yang digunakan untuk merepresentasikan string Teks. |
| [setVal(String value)](#setVal-java.lang.String-) | Mengatur nilai aktual dalam representasi internal. |
### Value() {#Value--}
```
public Value()
```


Menginisialisasi instance baru dari kelas [Value](../../com.aspose/tasks/value).

### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Mendapatkan nilai aktual jika dapat direpresentasikan sebagai DateTime. Nilai default adalah DateTime\#MinValue.MinValue.

--------------------

Lebih disarankan menggunakan properti ini daripada `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), ketika Anda perlu mengatur nilai DateTime.

**Returns:**
java.util.Date - nilai sebenarnya jika dapat direpresentasikan sebagai DateTime.
### getDescription() {#getDescription--}
```
public final String getDescription()
```


Mendapatkan deskripsi dari sebuah nilai.

**Returns:**
java.lang.String - deskripsi sebuah nilai.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Mendapatkan nilai aktual yang digunakan untuk merepresentasikan Durasi.

--------------------

Lebih disarankan menggunakan properti ini daripada `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), ketika Anda perlu mengatur nilai Duration.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the actual value which is used to represent Duration.
### getId() {#getId--}
```
public final int getId()
```


Mendapatkan pengidentifikasi unik dari sebuah nilai di seluruh proyek.

Penting untuk tidak memiliki identifier yang sama untuk instance [Value](../../com.aspose.tasks/value) yang berbeda.

Nilai minimal `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) adalah `1`.

**Returns:**
int - identifier unik sebuah nilai di seluruh proyek.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Mendapatkan nilai aktual yang digunakan untuk merepresentasikan nilai angka atau biaya.

--------------------

Lebih disarankan menggunakan properti ini daripada `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), ketika Anda perlu mengatur nilai Number atau Cost.

**Returns:**
java.math.BigDecimal - nilai sebenarnya yang digunakan untuk merepresentasikan nilai number atau cost.
### getPhonetic() {#getPhonetic--}
```
public final String getPhonetic()
```


Mendapatkan informasi fonetik tentang nama bidang khusus.

**Returns:**
java.lang.String - informasi fonetik tentang nama bidang khusus.
### getStringValue() {#getStringValue--}
```
public final String getStringValue()
```


Mendapatkan nilai aktual yang digunakan untuk merepresentasikan string Teks.

--------------------

Lebih disarankan menggunakan properti ini daripada `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), ketika Anda perlu mengatur nilai Text.

**Returns:**
java.lang.String - nilai sebenarnya yang digunakan untuk merepresentasikan string Text.
### getVal() {#getVal--}
```
public final String getVal()
```


Mendapatkan nilai sebenarnya dalam representasi internal. Lebih disarankan menggunakan properti bertipe kuat yang tercantum di bawah.

--------------------

Jika Anda ingin mengatur nilai Text, lebih disarankan menggunakan properti bertipe kuat `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)).

Jika Anda ingin mengatur nilai Number atau Cost, lebih disarankan menggunakan properti bertipe kuat `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)).

Jika Anda ingin mengatur nilai Date/Start/Finish, lebih disarankan menggunakan properti bertipe kuat `DateValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)).

Jika Anda ingin mengatur nilai Duration, lebih disarankan menggunakan properti bertipe kuat `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)).

Jika tipe Anda tidak tercantum, gunakan properti `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)).

**Returns:**
java.lang.String - nilai sebenarnya dalam representasi internal.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


Mendapatkan GUID yang mengidentifikasi nilai ini di antara yang lain dalam seluruh proyek.

**Returns:**
java.util.UUID - GUID yang mengidentifikasi nilai ini di antara nilai lain dalam seluruh proyek.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Mengatur nilai sebenarnya jika dapat direpresentasikan sebagai DateTime. Nilai default adalah DateTime\#MinValue.MinValue.

--------------------

Lebih disarankan menggunakan properti ini daripada `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), ketika Anda perlu mengatur nilai DateTime.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | nilai sebenarnya jika dapat direpresentasikan sebagai DateTime. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


Mengatur deskripsi dari sebuah nilai.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | deskripsi sebuah nilai. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Mengatur nilai aktual yang digunakan untuk merepresentasikan Durasi.

--------------------

Lebih disarankan menggunakan properti ini daripada `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), ketika Anda perlu mengatur nilai Duration.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | nilai sebenarnya yang digunakan untuk merepresentasikan Duration. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Mengatur pengidentifikasi unik dari sebuah nilai di seluruh proyek.

Penting untuk tidak memiliki identifier yang sama untuk instance [Value](../../com.aspose.tasks/value) yang berbeda.

Nilai minimal `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) adalah `1`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | pengidentifikasi unik dari sebuah nilai di seluruh proyek. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Mengatur nilai aktual yang digunakan untuk merepresentasikan nilai angka atau biaya.

--------------------

Lebih disarankan menggunakan properti ini daripada `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), ketika Anda perlu mengatur nilai Number atau Cost.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.math.BigDecimal | nilai sebenarnya yang digunakan untuk merepresentasikan angka atau nilai biaya. |

### setPhonetic(String value) {#setPhonetic-java.lang.String-}
```
public final void setPhonetic(String value)
```


Mengatur informasi fonetik tentang nama bidang khusus.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | informasi fonetik tentang nama bidang kustom. |

### setStringValue(String value) {#setStringValue-java.lang.String-}
```
public final void setStringValue(String value)
```


Mengatur nilai aktual yang digunakan untuk merepresentasikan string Teks.

--------------------

Lebih disarankan menggunakan properti ini daripada `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), ketika Anda perlu mengatur nilai Text.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai sebenarnya yang digunakan untuk merepresentasikan string Teks. |

### setVal(String value) {#setVal-java.lang.String-}
```
public final void setVal(String value)
```


Mengatur nilai sebenarnya dalam representasi internal. Lebih baik menggunakan properti bertipe kuat yang tercantum di bawah.

--------------------

Jika Anda ingin mengatur nilai Text, lebih disarankan menggunakan properti bertipe kuat `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)).

Jika Anda ingin mengatur nilai Number atau Cost, lebih disarankan menggunakan properti bertipe kuat `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)).

Jika Anda ingin mengatur nilai Date/Start/Finish, lebih baik menggunakan properti bertipe kuat `DateTimeValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)).

Jika Anda ingin mengatur nilai Duration, lebih disarankan menggunakan properti bertipe kuat `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)).

Jika tipe Anda tidak tercantum, gunakan properti `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai sebenarnya dalam representasi internal. |

