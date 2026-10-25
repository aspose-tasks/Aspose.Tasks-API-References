---
title: "Değer"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir değer listesindeki bir değeri temsil eder."
type: docs
weight: 333
url: /tr/java/com.aspose.tasks/value/
---

**Inheritance:**
java.lang.Object
```
public class Value
```

Bir değer listesindeki bir değeri temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Value()](#Value--) | Yeni bir [Değer](../../com.aspose.tasks/value) sınıfının örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getDateValue()](#getDateValue--) | DateTime olarak temsil edilebiliyorsa gerçek değeri alır. |
| [getDescription()](#getDescription--) | Bir değerin açıklamasını alır. |
| [getDuration()](#getDuration--) | Süreyi temsil etmek için kullanılan gerçek değeri alır. |
| [getId()](#getId--) | Bir proje genelinde bir değerin benzersiz tanımlayıcısını alır. |
| [getNumericValue()](#getNumericValue--) | Sayı veya maliyet değerini temsil etmek için kullanılan gerçek değeri alır. |
| [getPhonetic()](#getPhonetic--) | Özel alan adıyla ilgili fonetik bilgileri alır. |
| [getStringValue()](#getStringValue--) | Metin dizesini temsil etmek için kullanılan gerçek değeri alır. |
| [getVal()](#getVal--) | İç temsildeki gerçek değeri alır. |
| [getValueGuid()](#getValueGuid--) | Tüm projedeki diğer değerler arasında bu değeri tanımlayan bir GUID alır. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | DateTime olarak temsil edilebiliyorsa gerçek değeri ayarlar. |
| [setDescription(String value)](#setDescription-java.lang.String-) | Bir değerin açıklamasını ayarlar. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Süreyi temsil etmek için kullanılan gerçek değeri ayarlar. |
| [setId(int value)](#setId-int-) | Bir proje genelinde bir değerin benzersiz tanımlayıcısını ayarlar. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Sayı veya maliyet değerini temsil etmek için kullanılan gerçek değeri ayarlar. |
| [setPhonetic(String value)](#setPhonetic-java.lang.String-) | Özel alan adıyla ilgili fonetik bilgileri ayarlar. |
| [setStringValue(String value)](#setStringValue-java.lang.String-) | Metin dizesini temsil etmek için kullanılan gerçek değeri ayarlar. |
| [setVal(String value)](#setVal-java.lang.String-) | İç temsildeki gerçek değeri ayarlar. |
### Value() {#Value--}
```
public Value()
```


Yeni bir [Değer](../../com.aspose.tasks/value) sınıfının örneğini başlatır.

### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


DateTime olarak temsil edilebiliyorsa gerçek değeri alır. Varsayılan değer DateTime\#MinValue.MinValue'dir.

--------------------

DateTime değerini ayarlamanız gerektiğinde, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) yerine bu özelliği tercih edin.

**Returns:**
java.util.Date - DateTime olarak temsil edilebiliyorsa gerçek değer.
### getDescription() {#getDescription--}
```
public final String getDescription()
```


Bir değerin açıklamasını alır.

**Returns:**
java.lang.String - bir değerin açıklaması.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Süreyi temsil etmek için kullanılan gerçek değeri alır.

--------------------

Duration değerini ayarlamanız gerektiğinde, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) yerine bu özelliği tercih edin.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the actual value which is used to represent Duration.
### getId() {#getId--}
```
public final int getId()
```


Bir proje genelinde bir değerin benzersiz tanımlayıcısını alır.

Farklı [Value](../../com.aspose.tasks/value) örnekleri için aynı tanımlayıcıların olmaması önemlidir.

Minimum `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) değeri `1`'dir.

**Returns:**
int - bir proje boyunca bir değerin benzersiz tanımlayıcısı.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Sayı veya maliyet değerini temsil etmek için kullanılan gerçek değeri alır.

--------------------

Number veya Cost değerini ayarlamanız gerektiğinde, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) yerine bu özelliği tercih edin.

**Returns:**
java.math.BigDecimal - sayı veya maliyet değerini temsil etmek için kullanılan gerçek değer.
### getPhonetic() {#getPhonetic--}
```
public final String getPhonetic()
```


Özel alan adıyla ilgili fonetik bilgileri alır.

**Returns:**
java.lang.String - özel alan adıyla ilgili fonetik bilgi.
### getStringValue() {#getStringValue--}
```
public final String getStringValue()
```


Metin dizesini temsil etmek için kullanılan gerçek değeri alır.

--------------------

Text değerini ayarlamanız gerektiğinde, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) yerine bu özelliği tercih edin.

**Returns:**
java.lang.String - Text dizesini temsil etmek için kullanılan gerçek değer.
### getVal() {#getVal--}
```
public final String getVal()
```


İç temsildeki gerçek değeri alır. Aşağıda listelenen güçlü tipli özellikleri kullanmayı tercih edin.

--------------------

Text değerini ayarlamak istiyorsanız, güçlü tipli `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)) özelliğini kullanmayı tercih edin.

Number veya Cost değerini ayarlamak istiyorsanız, güçlü tipli `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)) özelliğini kullanmayı tercih edin.

Date/Start/Finish değerlerini ayarlamak istiyorsanız, güçlü tipli `DateValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)) özelliğini kullanmayı tercih edin.

Duration değerini ayarlamak istiyorsanız, güçlü tipli `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)) özelliğini kullanmayı tercih edin.

Tipiniz listelenmemişse, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) özelliğini kullanın.

**Returns:**
java.lang.String - iç temsildeki gerçek değer.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


Tüm projedeki diğer değerler arasında bu değeri tanımlayan bir GUID alır.

**Returns:**
java.util.UUID - tüm projedeki diğer değerler arasında bu değeri tanımlayan bir GUID.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


DateTime olarak temsil edilebiliyorsa gerçek değeri ayarlar. Varsayılan değer DateTime\#MinValue.MinValue'dir.

--------------------

DateTime değerini ayarlamanız gerektiğinde, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) yerine bu özelliği tercih edin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | DateTime olarak temsil edilebiliyorsa gerçek değer. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


Bir değerin açıklamasını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | bir değerin açıklaması. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Süreyi temsil etmek için kullanılan gerçek değeri ayarlar.

--------------------

Duration değerini ayarlamanız gerektiğinde, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) yerine bu özelliği tercih edin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Duration'ı temsil etmek için kullanılan gerçek değer. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Bir proje genelinde bir değerin benzersiz tanımlayıcısını ayarlar.

Farklı [Value](../../com.aspose.tasks/value) örnekleri için aynı tanımlayıcıların olmaması önemlidir.

Minimum `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) değeri `1`'dir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | bir proje genelinde bir değerin benzersiz tanımlayıcısı. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Sayı veya maliyet değerini temsil etmek için kullanılan gerçek değeri ayarlar.

--------------------

Number veya Cost değerini ayarlamanız gerektiğinde, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) yerine bu özelliği tercih edin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | sayı veya maliyet değerini temsil etmek için kullanılan gerçek değer. |

### setPhonetic(String value) {#setPhonetic-java.lang.String-}
```
public final void setPhonetic(String value)
```


Özel alan adıyla ilgili fonetik bilgileri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | özel alan adıyla ilgili fonetik bilgi. |

### setStringValue(String value) {#setStringValue-java.lang.String-}
```
public final void setStringValue(String value)
```


Metin dizesini temsil etmek için kullanılan gerçek değeri ayarlar.

--------------------

Text değerini ayarlamanız gerektiğinde, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) yerine bu özelliği tercih edin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Metin dizesini temsil etmek için kullanılan gerçek değer. |

### setVal(String value) {#setVal-java.lang.String-}
```
public final void setVal(String value)
```


İç temsilde gerçek değeri ayarlar. Aşağıda listelenen güçlü tipli özellikleri kullanmayı tercih edin.

--------------------

Text değerini ayarlamak istiyorsanız, güçlü tipli `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)) özelliğini kullanmayı tercih edin.

Number veya Cost değerini ayarlamak istiyorsanız, güçlü tipli `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)) özelliğini kullanmayı tercih edin.

Date/Start/Finish değerlerini ayarlamak istiyorsanız, güçlü tipli `DateTimeValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)) özelliğini tercih edin.

Duration değerini ayarlamak istiyorsanız, güçlü tipli `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)) özelliğini kullanmayı tercih edin.

Tipiniz listelenmemişse, `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) özelliğini kullanın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | iç temsildeki gerçek değer. |

