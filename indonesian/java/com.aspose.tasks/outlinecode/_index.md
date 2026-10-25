---
title: "OutlineCode"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili nilai dari kode outline."
type: docs
weight: 167
url: /id/java/com.aspose.tasks/outlinecode/
---

**Inheritance:**
java.lang.Object
```
public class OutlineCode
```

Mewakili nilai dari kode outline.

--------------------

Dua potongan data diperlukan - pointer ke tabel kode outline yang ditentukan oleh FieldId, dan nilai yang ditentukan baik oleh ValueId atau pointer ValueGuid ke daftar nilai.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [OutlineCode()](#OutlineCode--) | Menginisialisasi instance baru dari kelas [OutlineCode](../../com.aspose.tasks/outlinecode). |
| [OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)](#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-) | Menginisialisasi instance baru dari kelas [OutlineCode](../../com.aspose.tasks/outlinecode) menggunakan Outline Code yang ditentukan dan salah satu nilainya. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getFieldId()](#getFieldId--) | Mengambil nilai numerik dari bidang khusus Id proyek. |
| [getValueGuid()](#getValueGuid--) | Mengambil GUID dari nilai dalam daftar nilai. |
| [getValueId()](#getValueId--) | Mengambil Id dalam daftar nilai yang terkait dengan definisi dalam koleksi kode outline. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | Mengatur nilai numerik dari bidang khusus Id proyek. |
| [setValueGuid(String value)](#setValueGuid-java.lang.String-) | Mengatur GUID dari nilai dalam daftar nilai. |
| [setValueId(int value)](#setValueId-int-) | Mengatur Id dalam daftar nilai yang terkait dengan definisi dalam koleksi kode outline. |
### OutlineCode() {#OutlineCode--}
```
public OutlineCode()
```


Menginisialisasi instance baru dari kelas [OutlineCode](../../com.aspose.tasks/outlinecode).

### OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue) {#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-}
```
public OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)
```


Menginisialisasi instance baru dari kelas [OutlineCode](../../com.aspose.tasks/outlinecode) menggunakan Outline Code yang ditentukan dan salah satu nilainya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| codeDefinition | [OutlineCodeDefinition](../../com.aspose.tasks/outlinecodedefinition) | definisi kode outline. |
| outlineValue | [OutlineValue](../../com.aspose.tasks/outlinevalue) | salah satu nilai definisi kode outline. |

### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Mengambil nilai numerik dari bidang khusus Id proyek.

**Returns:**
java.lang.String - nilai angka dari bidang khusus Id proyek.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


Mendapatkan GUID dari nilai dalam daftar nilai. ValueGuid cocok dengan FieldGuid dalam daftar nilai.

**Returns:**
java.lang.String - GUID dari nilai dalam daftar nilai.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


Mengambil Id dalam daftar nilai yang terkait dengan definisi dalam koleksi kode outline.

**Returns:**
int - Id dalam daftar nilai yang terkait dengan definisi dalam koleksi kode outline.
### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


Mengatur nilai numerik dari bidang khusus Id proyek.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai angka dari bidang khusus Id proyek. |

### setValueGuid(String value) {#setValueGuid-java.lang.String-}
```
public final void setValueGuid(String value)
```


Mengatur GUID dari nilai dalam daftar nilai. ValueGuid cocok dengan FieldGuid dalam daftar nilai.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | GUID dari nilai dalam daftar nilai. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


Mengatur Id dalam daftar nilai yang terkait dengan definisi dalam koleksi kode outline.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | Id dalam daftar nilai yang terkait dengan definisi dalam koleksi kode outline. |

