---
title: "TimephasedData"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili data berfase waktu."
type: docs
weight: 320
url: /id/java/com.aspose.tasks/timephaseddata/
---

**Inheritance:**
java.lang.Object
```
public class TimephasedData
```

Mewakili data berfase waktu.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [TimephasedData()](#TimephasedData--) | Menginisialisasi instance baru dari kelas [TimephasedData](../../com.aspose.tasks/timephaseddata). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-) | Membuat dan menginisialisasi instance baru dari kelas [TimephasedData](../../com.aspose.tasks/timephaseddata) untuk data berwaktu berbasis biaya. |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Membuat dan menginisialisasi instance baru dari kelas [TimephasedData](../../com.aspose.tasks/timephaseddata) untuk data berwaktu berbasis biaya. |
| [createUnitTimephased(int uid, Date start, Date finish, double units, byte type)](#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-) | Membuat dan menginisialisasi instance baru dari kelas [TimephasedData](../../com.aspose.tasks/timephaseddata) untuk data berwaktu berbasis unit dari penugasan sumber daya material. |
| [createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Membuat dan menginisialisasi instance baru dari kelas [TimephasedData](../../com.aspose.tasks/timephaseddata) untuk data berwaktu berbasis kerja. |
| [getFinish()](#getFinish--) | Mendapatkan tanggal selesai dari periode data berwaktu. |
| [getStart()](#getStart--) | Mendapatkan tanggal mulai dari periode data berwaktu. |
| [getTimephasedDataType()](#getTimephasedDataType--) | Mendapatkan tipe dari data berwaktu. |
| [getUid()](#getUid--) | Mendapatkan pengidentifikasi unik dari data berwaktu |
| [getUnit()](#getUnit--) | Mendapatkan satuan waktu dari periode data berwaktu. |
| [getValue()](#getValue--) | Mendapatkan nilai per satuan waktu untuk periode data berwaktu. |
| [getValueToCost()](#getValueToCost--) | Mendapatkan instance `double` yang merepresentasikan nilai string dari objek ini. |
| [getValueToDuration()](#getValueToDuration--) | Mendapatkan instance double yang merepresentasikan nilai string dari objek ini. |
| [getValueToUnits()](#getValueToUnits--) | Mendapatkan instance `double` yang merepresentasikan nilai string dari objek ini untuk data berwaktu berbasis unit. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Mengatur tanggal selesai dari periode data berwaktu. |
| [setStart(Date value)](#setStart-java.util.Date-) | Mengatur tanggal mulai dari periode data berwaktu. |
| [setTimephasedDataType(byte value)](#setTimephasedDataType-byte-) | Mengatur tipe dari data berwaktu. |
| [setUid(int value)](#setUid-int-) | Mengatur pengidentifikasi unik dari data berwaktu |
| [setUnit(byte value)](#setUnit-byte-) | Mengatur satuan waktu dari periode data berwaktu. |
| [setValue(String value)](#setValue-java.lang.String-) | Mengatur nilai per satuan waktu untuk periode data berwaktu. |
| [setValueToCost(double value)](#setValueToCost-double-) | Instance `double` yang merepresentasikan nilai string dari objek ini. |
### TimephasedData() {#TimephasedData--}
```
public TimephasedData()
```


Menginisialisasi instance baru dari kelas [TimephasedData](../../com.aspose.tasks/timephaseddata).

### createCostTimephased(int uid, Date start, Date finish, double value, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte type)
```


Membuat dan menginisialisasi instance baru dari kelas [TimephasedData](../../com.aspose.tasks/timephaseddata) untuk data berwaktu berbasis biaya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| uid | int | UID dari tugas. |
| mulai | java.util.Date | tanggal-waktu mulai. |
| selesai | java.util.Date | Tanggal-waktu selesai. |
| nilai | double | Nilai biaya. |
| type | byte | Tipe data berwaktu. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Membuat dan menginisialisasi instance baru dari kelas [TimephasedData](../../com.aspose.tasks/timephaseddata) untuk data berwaktu berbasis biaya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| uid | int | UID dari tugas. |
| mulai | java.util.Date | tanggal-waktu mulai. |
| selesai | java.util.Date | Tanggal-waktu selesai. |
| nilai | double | Nilai biaya. |
| timeUnit | byte | Tipe satuan waktu. |
| type | byte | Tipe data berwaktu. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createUnitTimephased(int uid, Date start, Date finish, double units, byte type) {#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createUnitTimephased(int uid, Date start, Date finish, double units, byte type)
```


Membuat dan menginisialisasi instance baru dari kelas [TimephasedData](../../com.aspose.tasks/timephaseddata) untuk data berwaktu berbasis unit dari penugasan sumber daya material.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| uid | int | UID dari tugas. |
| mulai | java.util.Date | Tanggal dan waktu mulai. |
| selesai | java.util.Date | Tanggal-waktu selesai. |
| unit | double | Jumlah unit. |
| type | byte | Tipe data berwaktu. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Membuat dan menginisialisasi instance baru dari kelas [TimephasedData](../../com.aspose.tasks/timephaseddata) untuk data berwaktu berbasis kerja.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| uid | int | UID dari tugas. |
| mulai | java.util.Date | tanggal-waktu mulai. |
| selesai | java.util.Date | Tanggal-waktu selesai. |
| nilai | double | Nilai rentang waktu. |
| timeUnit | byte | Tipe satuan waktu. |
| type | byte | Tipe data berwaktu. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for work-based time phased data.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Mendapatkan tanggal selesai dari periode data berwaktu.

**Returns:**
java.util.Date - tanggal selesai dari periode data berfase waktu.
### getStart() {#getStart--}
```
public final Date getStart()
```


Mendapatkan tanggal mulai dari periode data berwaktu.

**Returns:**
java.util.Date - tanggal mulai dari periode data berfase waktu.
### getTimephasedDataType() {#getTimephasedDataType--}
```
public final byte getTimephasedDataType()
```


Mendapatkan tipe dari data berwaktu.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) properti akan dibersihkan, jika tidak cocok untuk tipe, yang ditentukan di sini.

**Returns:**
byte - tipe data berfase waktu.
### getUid() {#getUid--}
```
public final int getUid()
```


Mendapatkan pengidentifikasi unik dari data berwaktu

**Returns:**
int - pengidentifikasi unik dari data berfase waktu
### getUnit() {#getUnit--}
```
public final byte getUnit()
```


Mendapatkan satuan waktu dari periode data berwaktu.

**Returns:**
byte - satuan waktu dari periode data berfase waktu.
### getValue() {#getValue--}
```
public final String getValue()
```


Mendapatkan nilai per satuan waktu untuk periode data berwaktu.

**Returns:**
java.lang.String - nilai per satuan waktu untuk periode data berfase waktu.
### getValueToCost() {#getValueToCost--}
```
public final double getValueToCost()
```


Mendapatkan instance `double` yang merepresentasikan nilai string dari objek ini.

**Returns:**
double - representasi titik mengambang dari objek.
### getValueToDuration() {#getValueToDuration--}
```
public final double getValueToDuration()
```


Mendapatkan instance double yang merepresentasikan nilai string dari objek ini.

**Returns:**
double - representasi rentang waktu dari objek.
### getValueToUnits() {#getValueToUnits--}
```
public final double getValueToUnits()
```


Mendapatkan instance `double` yang merepresentasikan nilai string dari objek ini untuk data berwaktu berbasis unit.

**Returns:**
double - representasi titik mengambang dari objek ini.
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Mengatur tanggal selesai dari periode data berwaktu.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | tanggal selesai dari periode data berfase waktu. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Mengatur tanggal mulai dari periode data berwaktu.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | tanggal mulai dari periode data berfase waktu. |

### setTimephasedDataType(byte value) {#setTimephasedDataType-byte-}
```
public final void setTimephasedDataType(byte value)
```


Mengatur tipe dari data berwaktu.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) properti akan dibersihkan, jika tidak cocok untuk tipe, yang ditentukan di sini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | byte | tipe data berfase waktu. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Mengatur pengidentifikasi unik dari data berwaktu

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | pengidentifikasi unik dari data berfase waktu |

### setUnit(byte value) {#setUnit-byte-}
```
public final void setUnit(byte value)
```


Mengatur satuan waktu dari periode data berwaktu.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | byte | satuan waktu dari periode data berfase waktu. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


Mengatur nilai per satuan waktu untuk periode data berwaktu.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai per satuan waktu untuk periode data berfase waktu. |

### setValueToCost(double value) {#setValueToCost-double-}
```
public final void setValueToCost(double value)
```


Instance `double` yang merepresentasikan nilai string dari objek ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | Instance `double` yang merepresentasikan nilai string dari objek ini. |

