---
title: "ExtendedAttribute"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili atribut tambahan."
type: docs
weight: 81
url: /id/java/com.aspose.tasks/extendedattribute/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttribute
```

Mewakili atribut tambahan.

--------------------

Saat ini mendukung semua jenis atribut Extended yang dibaca dari MSP Xml 2003/2007 dan mpp 2003. Untuk MSP mpp 2007 semua pembacaan atribut Extended didukung kecuali durasi dan flag.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getAttributeDefinition()](#getAttributeDefinition--) | Mendapatkan definisi atribut. |
| [getDateValue()](#getDateValue--) | Mendapatkan nilai untuk atribut dengan tipe tanggal (Date, Start, Finish). |
| [getDurationValue()](#getDurationValue--) | Mendapatkan nilai untuk atribut dengan tipe 'Duration'. |
| [getFieldId()](#getFieldId--) | Mendapatkan id dari sebuah field. |
| [getFlagValue()](#getFlagValue--) | Mendapatkan nilai yang menunjukkan apakah sebuah flag diatur untuk atribut dengan tipe 'Flag'. |
| [getNumericValue()](#getNumericValue--) | Mendapatkan nilai untuk atribut dengan tipe numerik (Cost, Number). |
| [getTextValue()](#getTextValue--) | Mendapatkan nilai untuk atribut dengan tipe 'Text'. |
| [getValueGuid()](#getValueGuid--) | Mendapatkan guid dari nilai lookup. |
| [getValueReadOnly()](#getValueReadOnly--) | Mendapatkan nilai yang menunjukkan apakah nilai dari instance [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) ini bersifat read-only. |
| [isErrorValue()](#isErrorValue--) | Mendapatkan apakah perhitungan nilai extended attribute menghasilkan error. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Mengatur nilai untuk atribut dengan tipe tanggal (Date, Start, Finish). |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | Mengatur nilai untuk atribut dengan tipe 'Duration'. |
| [setFlagValue(boolean value)](#setFlagValue-boolean-) | Mengatur nilai yang menunjukkan apakah sebuah flag diatur untuk atribut dengan tipe 'Flag'. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Mengatur nilai untuk atribut dengan tipe numerik (Cost, Number). |
| [setTextValue(String value)](#setTextValue-java.lang.String-) | Mengatur nilai untuk atribut dengan tipe 'Text'. |
| [toString()](#toString--) | Mengembalikan representasi string pendek dari sebuah extended attribute. |
### getAttributeDefinition() {#getAttributeDefinition--}
```
public final ExtendedAttributeDefinition getAttributeDefinition()
```


Mendapatkan definisi atribut.

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - the attribute definition.
### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Mendapatkan nilai untuk atribut dengan tipe tanggal (Date, Start, Finish).

**Returns:**
java.util.Date - nilai untuk atribut dengan tipe tanggal (Date, Start, Finish).
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


Mendapatkan nilai untuk atribut dengan tipe 'Duration'.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - value for attributes with 'Duration' type.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Mendapatkan id dari sebuah field.

**Returns:**
java.lang.String - id dari sebuah field.
### getFlagValue() {#getFlagValue--}
```
public final boolean getFlagValue()
```


Mendapatkan nilai yang menunjukkan apakah sebuah flag diatur untuk atribut dengan tipe 'Flag'.

**Returns:**
boolean - nilai yang menunjukkan apakah sebuah flag diatur untuk atribut dengan tipe 'Flag'.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Mendapatkan nilai untuk atribut dengan tipe numerik (Cost, Number).

**Returns:**
java.math.BigDecimal - nilai untuk atribut dengan tipe numerik (Cost, Number).
### getTextValue() {#getTextValue--}
```
public final String getTextValue()
```


Mendapatkan nilai untuk atribut dengan tipe 'Text'.

**Returns:**
java.lang.String - nilai untuk atribut dengan tipe 'Text'.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


Mendapatkan guid dari nilai lookup.

--------------------

Tidak boleh diatur secara langsung, gunakan ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) untuk membuat extended attribute dengan nilai lookup.

**Returns:**
java.lang.String - guid dari nilai lookup.
### getValueReadOnly() {#getValueReadOnly--}
```
public final boolean getValueReadOnly()
```


Mendapatkan nilai yang menunjukkan apakah nilai dari instance [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) ini bersifat read-only.

Value: mengembalikan true jika sebuah formula atau rollup didefinisikan dalam [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) untuk objek ini.

**Returns:**
boolean - nilai yang menunjukkan apakah nilai dari instance [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) ini bersifat read-only.
### isErrorValue() {#isErrorValue--}
```
public final boolean isErrorValue()
```


Mendapatkan apakah perhitungan nilai extended attribute menghasilkan error.

**Returns:**
boolean - apakah perhitungan nilai extended attribute menghasilkan error.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Mengatur nilai untuk atribut dengan tipe tanggal (Date, Start, Finish).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | nilai untuk atribut dengan tipe tanggal (Date, Start, Finish). |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


Mengatur nilai untuk atribut dengan tipe 'Duration'.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | nilai untuk atribut dengan tipe 'Duration'. |

### setFlagValue(boolean value) {#setFlagValue-boolean-}
```
public final void setFlagValue(boolean value)
```


Mengatur nilai yang menunjukkan apakah sebuah flag diatur untuk atribut dengan tipe 'Flag'.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah flag sudah diatur untuk atribut dengan tipe 'Flag'. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Mengatur nilai untuk atribut dengan tipe numerik (Cost, Number).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.math.BigDecimal | nilai untuk atribut dengan tipe numerik (Cost, Number). |

### setTextValue(String value) {#setTextValue-java.lang.String-}
```
public final void setTextValue(String value)
```


Mengatur nilai untuk atribut dengan tipe 'Text'.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai untuk atribut dengan tipe 'Text'. |

### toString() {#toString--}
```
public String toString()
```


Mengembalikan representasi string pendek dari sebuah extended attribute.

**Returns:**
java.lang.String - Representasi string dari atribut yang diperluas.
