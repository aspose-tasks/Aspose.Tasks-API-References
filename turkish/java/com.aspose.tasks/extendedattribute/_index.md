---
title: "ExtendedAttribute"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Genişletilmiş öznitelikleri temsil eder."
type: docs
weight: 81
url: /tr/java/com.aspose.tasks/extendedattribute/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttribute
```

Genişletilmiş öznitelikleri temsil eder.

--------------------

Şu anda MSP Xml 2003/2007 ve mpp 2003'ten Extended attribute'ların tüm türlerinin okunması desteklenmektedir. MSP mpp 2007 için ise tüm Extended attribute okumaları desteklenmektedir, ancak süreler ve bayraklar hariçtir.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getAttributeDefinition()](#getAttributeDefinition--) | Özellik tanımını alır. |
| [getDateValue()](#getDateValue--) | Tarih türündeki (Date, Start, Finish) özellikler için bir değer alır. |
| [getDurationValue()](#getDurationValue--) | ‘Duration’ türündeki öznitelikler için değeri alır. |
| [getFieldId()](#getFieldId--) | Bir alanın kimliğini alır. |
| [getFlagValue()](#getFlagValue--) | ‘Flag’ türündeki bir öznitelik için bayrağın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [getNumericValue()](#getNumericValue--) | Sayısal türdeki (Cost, Number) öznitelikler için bir değer alır. |
| [getTextValue()](#getTextValue--) | ‘Text’ türündeki öznitelikler için bir değer alır. |
| [getValueGuid()](#getValueGuid--) | Bir arama değerinin GUID'sini alır. |
| [getValueReadOnly()](#getValueReadOnly--) | Bu [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) örneğinin değerinin yalnızca okunur olup olmadığını gösteren bir değer alır. |
| [isErrorValue()](#isErrorValue--) | Genişletilmiş öznitelik değerinin hesaplamasının bir hatayla sonuçlanıp sonuçlanmadığını alır. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Tarih türündeki (Date, Start, Finish) öznitelikler için bir değer ayarlar. |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | ‘Duration’ türündeki öznitelikler için değeri ayarlar. |
| [setFlagValue(boolean value)](#setFlagValue-boolean-) | ‘Flag’ türündeki bir öznitelik için bayrağın ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Sayısal türdeki (Cost, Number) öznitelikler için bir değer ayarlar. |
| [setTextValue(String value)](#setTextValue-java.lang.String-) | ‘Text’ türündeki öznitelikler için bir değer ayarlar. |
| [toString()](#toString--) | Genişletilmiş bir özniteliğin kısa dize temsilini döndürür. |
### getAttributeDefinition() {#getAttributeDefinition--}
```
public final ExtendedAttributeDefinition getAttributeDefinition()
```


Özellik tanımını alır.

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - the attribute definition.
### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Tarih türündeki (Date, Start, Finish) özellikler için bir değer alır.

**Returns:**
java.util.Date - tarih türündeki (Date, Start, Finish) öznitelikler için bir değer.
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


‘Duration’ türündeki öznitelikler için değeri alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - value for attributes with 'Duration' type.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Bir alanın kimliğini alır.

**Returns:**
java.lang.String - bir alanın kimliği.
### getFlagValue() {#getFlagValue--}
```
public final boolean getFlagValue()
```


‘Flag’ türündeki bir öznitelik için bayrağın ayarlanıp ayarlanmadığını gösteren bir değer alır.

**Returns:**
boolean - ‘Flag’ türündeki bir öznitelik için bayrağın ayarlanıp ayarlanmadığını gösteren bir değer.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Sayısal türdeki (Cost, Number) öznitelikler için bir değer alır.

**Returns:**
java.math.BigDecimal - sayısal türdeki (Cost, Number) öznitelikler için bir değer.
### getTextValue() {#getTextValue--}
```
public final String getTextValue()
```


‘Text’ türündeki öznitelikler için bir değer alır.

**Returns:**
java.lang.String - ‘Text’ türündeki öznitelikler için bir değer.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


Bir arama değerinin GUID'sini alır.

--------------------

Doğrudan ayarlanmamalıdır, bunun yerine bir arama değeriyle genişletilmiş bir öznitelik oluşturmak için ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) kullanın.

**Returns:**
java.lang.String - bir arama değerinin GUID'si.
### getValueReadOnly() {#getValueReadOnly--}
```
public final boolean getValueReadOnly()
```


Bu [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) örneğinin değerinin yalnızca okunur olup olmadığını gösteren bir değer alır.

Value: bu nesne için [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) içinde bir formül veya toplama tanımlıysa true döndürür.

**Returns:**
boolean - bu [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) örneğinin değerinin yalnızca okunur olup olmadığını gösteren bir değer.
### isErrorValue() {#isErrorValue--}
```
public final boolean isErrorValue()
```


Genişletilmiş öznitelik değerinin hesaplamasının bir hatayla sonuçlanıp sonuçlanmadığını alır.

**Returns:**
boolean - genişletilmiş öznitelik değerinin hesaplamasının bir hatayla sonuçlanıp sonuçlanmadığı.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Tarih türündeki (Date, Start, Finish) öznitelikler için bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | tarih türündeki (Date, Start, Finish) öznitelikler için bir değer. |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


‘Duration’ türündeki öznitelikler için değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | 'Duration' tipindeki öznitelikler için değer. |

### setFlagValue(boolean value) {#setFlagValue-boolean-}
```
public final void setFlagValue(boolean value)
```


‘Flag’ türündeki bir öznitelik için bayrağın ayarlanıp ayarlanmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | 'Flag' türündeki bir öznitelik için işaretin ayarlanıp ayarlanmadığını gösteren değer. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Sayısal türdeki (Cost, Number) öznitelikler için bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | Sayısal tipteki (Cost, Number) öznitelikler için değer. |

### setTextValue(String value) {#setTextValue-java.lang.String-}
```
public final void setTextValue(String value)
```


‘Text’ türündeki öznitelikler için bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | 'Text' türündeki öznitelikler için değer. |

### toString() {#toString--}
```
public String toString()
```


Genişletilmiş bir özniteliğin kısa dize temsilini döndürür.

**Returns:**
java.lang.String - Genişletilmiş özniteliğin dize temsili.
