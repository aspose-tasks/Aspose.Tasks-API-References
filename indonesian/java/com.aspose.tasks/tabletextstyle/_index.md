---
title: "TableTextStyle"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili gaya teks dalam tabel tampilan."
type: docs
weight: 288
url: /id/java/com.aspose.tasks/tabletextstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.TextStyle](../../com.aspose.tasks/textstyle)
```
public class TableTextStyle extends TextStyle
```

Mewakili gaya teks dalam tabel tampilan.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [TableTextStyle(int rowUid)](#TableTextStyle-int-) | Menginisialisasi instance baru dari kelas [TableTextStyle](../../com.aspose.tasks/tabletextstyle). |
| [TableTextStyle(int rowUid, FontDescriptor font)](#TableTextStyle-int-com.aspose.tasks.FontDescriptor-) | Menginisialisasi instance baru dari kelas [TableTextStyle](../../com.aspose.tasks/tabletextstyle) dengan font yang ditentukan. |
| [TableTextStyle(int rowUid, float fontSize, int fontStyle)](#TableTextStyle-int-float-int-) | Menginisialisasi instance baru dari kelas [TableTextStyle](../../com.aspose.tasks/tabletextstyle) dengan ukuran font dan gaya font yang ditentukan. |
| [TableTextStyle(int rowUid, int fontStyle)](#TableTextStyle-int-int-) | Menginisialisasi instance baru dari kelas [TableTextStyle](../../com.aspose.tasks/tabletextstyle) dengan pengaturan font default dan gaya font yang ditentukan. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getField()](#getField--) | Mendapatkan bidang yang akan diterapkan gaya. |
| [getItemType()](#getItemType--) | Mengembalikan tipe item teks. |
| [getRowUid()](#getRowUid--) | Mendapatkan id unik baris. |
| [setField(int value)](#setField-int-) | Mengatur bidang yang akan diterapkan gaya. |
### TableTextStyle(int rowUid) {#TableTextStyle-int-}
```
public TableTextStyle(int rowUid)
```


Menginisialisasi instance baru dari kelas [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| rowUid | int | Id unik baris yang ditentukan. |

### TableTextStyle(int rowUid, FontDescriptor font) {#TableTextStyle-int-com.aspose.tasks.FontDescriptor-}
```
public TableTextStyle(int rowUid, FontDescriptor font)
```


Menginisialisasi instance baru dari kelas [TableTextStyle](../../com.aspose.tasks/tabletextstyle) dengan font yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| rowUid | int | Id unik baris yang ditentukan. |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | Font yang menjadi dasar gaya teks. |

### TableTextStyle(int rowUid, float fontSize, int fontStyle) {#TableTextStyle-int-float-int-}
```
public TableTextStyle(int rowUid, float fontSize, int fontStyle)
```


Menginisialisasi instance baru dari kelas [TableTextStyle](../../com.aspose.tasks/tabletextstyle) dengan ukuran font dan gaya font yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| rowUid | int | Id unik baris yang ditentukan. |
| fontSize | float | Ukuran font yang menjadi dasar gaya teks. |
| fontStyle | int | Gaya font. |

### TableTextStyle(int rowUid, int fontStyle) {#TableTextStyle-int-int-}
```
public TableTextStyle(int rowUid, int fontStyle)
```


Menginisialisasi instance baru dari kelas [TableTextStyle](../../com.aspose.tasks/tabletextstyle) dengan pengaturan font default dan gaya font yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| rowUid | int | Id unik baris yang ditentukan. |
| fontStyle | int | Gaya font. |

### getField() {#getField--}
```
public final int getField()
```


Mendapatkan bidang yang akan diterapkan gaya. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Returns:**
int - bidang yang akan diterapkan gaya.
### getItemType() {#getItemType--}
```
public int getItemType()
```


Mengembalikan tipe item teks.

**Returns:**
int - nilai tipe enumerasi TextItemType.
### getRowUid() {#getRowUid--}
```
public final int getRowUid()
```


Mendapatkan id unik baris.

--------------------

Kembalikan -1 jika gaya akan diterapkan pada semua baris tampilan.

**Returns:**
int - ID unik baris.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Mengatur bidang yang akan diterapkan gaya. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | bidang yang akan diterapkan gaya. |

