---
title: "ViewColumn"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili kolom dalam tampilan proyek."
type: docs
weight: 344
url: /id/java/com.aspose.tasks/viewcolumn/
---

**Inheritance:**
java.lang.Object
```
public abstract class ViewColumn
```

Mewakili kolom dalam tampilan proyek.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getField()](#getField--) | Mendapatkan field kolom. |
| [getName()](#getName--) | Mendapatkan nama kolom. |
| [getStringAlignment()](#getStringAlignment--) | Mendapatkan perataan teks (bisa menjadi salah satu nilai dari enumerasi [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [getTextStyleModificationCallback()](#getTextStyleModificationCallback--) | Mendapatkan callback yang dapat digunakan untuk menyesuaikan tampilan sel kolom. |
| [getWidth()](#getWidth--) | Mendapatkan lebar kolom. |
| [setField(int value)](#setField-int-) | Mengatur bidang kolom. |
| [setStringAlignment(int value)](#setStringAlignment-int-) | Mengatur perataan teks (dapat menjadi salah satu nilai dari enumerasi [HorizontalStringAlignment](../../com.aspose/tasks/horizontalstringalignment)). |
| [setTextStyleModificationCallback(ITextStyleModificationCallback value)](#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-) | Mengatur callback yang dapat digunakan untuk menyesuaikan tampilan sel kolom. |
### getField() {#getField--}
```
public abstract int getField()
```


Mendapatkan bidang kolom. `Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Returns:**
int - bidang kolom.
### getName() {#getName--}
```
public final String getName()
```


Mendapatkan nama kolom.

**Returns:**
java.lang.String - nama kolom.
### getStringAlignment() {#getStringAlignment--}
```
public final int getStringAlignment()
```


Mendapatkan perataan teks (bisa menjadi salah satu nilai dari enumerasi [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Returns:**
int - perataan teks (dapat menjadi salah satu nilai dari enumerasi [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).
### getTextStyleModificationCallback() {#getTextStyleModificationCallback--}
```
public final ITextStyleModificationCallback getTextStyleModificationCallback()
```


Mendapatkan callback yang dapat digunakan untuk menyesuaikan tampilan sel kolom.

**Returns:**
[ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) - the callback which can be used to customize the appearance of the column's cells.
### getWidth() {#getWidth--}
```
public final int getWidth()
```


Mendapatkan lebar kolom.

**Returns:**
int - lebar kolom.
### setField(int value) {#setField-int-}
```
public abstract void setField(int value)
```


Mengatur bidang kolom. `Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | bidang kolom. |

### setStringAlignment(int value) {#setStringAlignment-int-}
```
public final void setStringAlignment(int value)
```


Mengatur perataan teks (dapat menjadi salah satu nilai dari enumerasi [HorizontalStringAlignment](../../com.aspose/tasks/horizontalstringalignment)).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | int | perataan teks (dapat menjadi salah satu nilai dari enumerasi [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |

### setTextStyleModificationCallback(ITextStyleModificationCallback value) {#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-}
```
public final void setTextStyleModificationCallback(ITextStyleModificationCallback value)
```


Mengatur callback yang dapat digunakan untuk menyesuaikan tampilan sel kolom.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) | callback yang dapat digunakan untuk menyesuaikan tampilan sel kolom. |

