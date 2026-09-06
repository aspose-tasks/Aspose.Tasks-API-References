---
title: "TimephasedData"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Zaman aşamalı bir veriyi temsil eder."
type: docs
weight: 320
url: /tr/java/com.aspose.tasks/timephaseddata/
---

**Inheritance:**
java.lang.Object
```
public class TimephasedData
```

Zaman aşamalı bir veriyi temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [TimephasedData()](#TimephasedData--) | Yeni bir [TimephasedData](../../com.aspose.tasks/timephaseddata) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-) | Maliyet temelli zaman aşamalı veri için yeni bir [TimephasedData](../../com.aspose.tasks/timephaseddata) sınıfının bir örneğini oluşturur ve başlatır. |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Maliyet temelli zaman aşamalı veri için yeni bir [TimephasedData](../../com.aspose.tasks/timephaseddata) sınıfının bir örneğini oluşturur ve başlatır. |
| [createUnitTimephased(int uid, Date start, Date finish, double units, byte type)](#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-) | Bir malzeme kaynağının atamasına ait birim temelli zaman aşamalı veri için yeni bir [TimephasedData](../../com.aspose.tasks/timephaseddata) sınıfının bir örneğini oluşturur ve başlatır. |
| [createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | İş temelli zaman aşamalı veri için yeni bir [TimephasedData](../../com.aspose.tasks/timephaseddata) sınıfının bir örneğini oluşturur ve başlatır. |
| [getFinish()](#getFinish--) | Bir zaman aşamalı veri dönemi için bitiş tarihini alır. |
| [getStart()](#getStart--) | Bir zaman aşamalı veri dönemi için başlangıç tarihini alır. |
| [getTimephasedDataType()](#getTimephasedDataType--) | Bir zaman aşamalı verinin türünü alır. |
| [getUid()](#getUid--) | Bir zaman aşamalı verinin benzersiz tanımlayıcısını alır |
| [getUnit()](#getUnit--) | Bir zaman aşamalı veri dönemi için zaman birimini alır. |
| [getValue()](#getValue--) | Bir zaman aşamalı veri dönemi için birim zaman başına değeri alır. |
| [getValueToCost()](#getValueToCost--) | `double` örneğini alır; bu örnek nesnenin dize değerini temsil eder. |
| [getValueToDuration()](#getValueToDuration--) | double örneğini alır; bu örnek nesnenin dize değerini temsil eder. |
| [getValueToUnits()](#getValueToUnits--) | Birim temelli zaman aşamalı veri için nesnenin dize değerini temsil eden `double` örneğini alır. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Bir zaman aşamalı veri dönemi için bitiş tarihini ayarlar. |
| [setStart(Date value)](#setStart-java.util.Date-) | Bir zaman aşamalı veri dönemi için başlangıç tarihini ayarlar. |
| [setTimephasedDataType(byte value)](#setTimephasedDataType-byte-) | Bir zaman aşamalı verinin türünü ayarlar. |
| [setUid(int value)](#setUid-int-) | Bir zaman aşamalı verinin benzersiz tanımlayıcısını ayarlar |
| [setUnit(byte value)](#setUnit-byte-) | Bir zaman aşamalı veri dönemi için zaman birimini ayarlar. |
| [setValue(String value)](#setValue-java.lang.String-) | Bir zaman aşamalı veri dönemi için birim zaman başına değeri ayarlar. |
| [setValueToCost(double value)](#setValueToCost-double-) | `double` örneği; bu örnek nesnenin dize değerini temsil eder. |
### TimephasedData() {#TimephasedData--}
```
public TimephasedData()
```


Yeni bir [TimephasedData](../../com.aspose.tasks/timephaseddata) sınıfı örneği başlatır.

### createCostTimephased(int uid, Date start, Date finish, double value, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte type)
```


Maliyet temelli zaman aşamalı veri için yeni bir [TimephasedData](../../com.aspose.tasks/timephaseddata) sınıfının bir örneğini oluşturur ve başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | int | Görevin UID'si. |
| başlat | java.util.Date | başlangıç tarih-saat. |
| bitiş | java.util.Date | Bitiş tarih-saat. |
| değer | double | Maliyet değeri. |
| tür | byte | Zaman aşamalı veri türü. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Maliyet temelli zaman aşamalı veri için yeni bir [TimephasedData](../../com.aspose.tasks/timephaseddata) sınıfının bir örneğini oluşturur ve başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | int | Görevin UID'si. |
| başlat | java.util.Date | başlangıç tarih-saat. |
| bitiş | java.util.Date | Bitiş tarih-saat. |
| değer | double | Maliyet değeri. |
| timeUnit | byte | Zaman birimi türü. |
| tür | byte | Zaman aşamalı veri türü. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createUnitTimephased(int uid, Date start, Date finish, double units, byte type) {#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createUnitTimephased(int uid, Date start, Date finish, double units, byte type)
```


Bir malzeme kaynağının atamasına ait birim temelli zaman aşamalı veri için yeni bir [TimephasedData](../../com.aspose.tasks/timephaseddata) sınıfının bir örneğini oluşturur ve başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | int | Görevin UID'si. |
| başlat | java.util.Date | Başlangıç tarih-saat. |
| bitiş | java.util.Date | Bitiş tarih-saat. |
| birimler | double | Birim sayısı. |
| tür | byte | Zaman aşamalı veri türü. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


İş temelli zaman aşamalı veri için yeni bir [TimephasedData](../../com.aspose.tasks/timephaseddata) sınıfının bir örneğini oluşturur ve başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | int | Görevin UID'si. |
| başlat | java.util.Date | başlangıç tarih-saat. |
| bitiş | java.util.Date | Bitiş tarih-saat. |
| değer | double | Zaman aralığı değeri. |
| timeUnit | byte | Zaman birimi türü. |
| tür | byte | Zaman aşamalı veri türü. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for work-based time phased data.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Bir zaman aşamalı veri dönemi için bitiş tarihini alır.

**Returns:**
java.util.Date - zaman aşamalı veri dönemi için bitiş tarihi.
### getStart() {#getStart--}
```
public final Date getStart()
```


Bir zaman aşamalı veri dönemi için başlangıç tarihini alır.

**Returns:**
java.util.Date - zaman aşamalı veri dönemi için başlangıç tarihi.
### getTimephasedDataType() {#getTimephasedDataType--}
```
public final byte getTimephasedDataType()
```


Bir zaman aşamalı verinin türünü alır.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) özelliği, burada belirtilen tipe uygun değilse temizlenecektir.

**Returns:**
byte - zaman aşamalı verinin türü.
### getUid() {#getUid--}
```
public final int getUid()
```


Bir zaman aşamalı verinin benzersiz tanımlayıcısını alır

**Returns:**
int - zaman aşamalı verinin benzersiz tanımlayıcısı
### getUnit() {#getUnit--}
```
public final byte getUnit()
```


Bir zaman aşamalı veri dönemi için zaman birimini alır.

**Returns:**
byte - zaman aşamalı veri döneminin zaman birimi.
### getValue() {#getValue--}
```
public final String getValue()
```


Bir zaman aşamalı veri dönemi için birim zaman başına değeri alır.

**Returns:**
java.lang.String - zaman aşamalı veri dönemi için birim zaman başına değer.
### getValueToCost() {#getValueToCost--}
```
public final double getValueToCost()
```


`double` örneğini alır; bu örnek nesnenin dize değerini temsil eder.

**Returns:**
double - nesnenin kayan nokta temsili.
### getValueToDuration() {#getValueToDuration--}
```
public final double getValueToDuration()
```


double örneğini alır; bu örnek nesnenin dize değerini temsil eder.

**Returns:**
double - nesnenin zaman aralığı temsili.
### getValueToUnits() {#getValueToUnits--}
```
public final double getValueToUnits()
```


Birim temelli zaman aşamalı veri için nesnenin dize değerini temsil eden `double` örneğini alır.

**Returns:**
double - bu nesnenin kayan nokta temsili.
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Bir zaman aşamalı veri dönemi için bitiş tarihini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | zaman aşamalı veri döneminin bitiş tarihi. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Bir zaman aşamalı veri dönemi için başlangıç tarihini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | zaman aşamalı veri döneminin başlangıç tarihi. |

### setTimephasedDataType(byte value) {#setTimephasedDataType-byte-}
```
public final void setTimephasedDataType(byte value)
```


Bir zaman aşamalı verinin türünü ayarlar.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) özelliği, burada belirtilen tipe uygun değilse temizlenecektir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte | zaman aşamalı verinin türü. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Bir zaman aşamalı verinin benzersiz tanımlayıcısını ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | zaman aşamalı verinin benzersiz tanımlayıcısı |

### setUnit(byte value) {#setUnit-byte-}
```
public final void setUnit(byte value)
```


Bir zaman aşamalı veri dönemi için zaman birimini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte | zaman aşamalı veri döneminin zaman birimi. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


Bir zaman aşamalı veri dönemi için birim zaman başına değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | zaman aşamalı veri dönemi için birim zaman başına değer. |

### setValueToCost(double value) {#setValueToCost-double-}
```
public final void setValueToCost(double value)
```


`double` örneği; bu örnek nesnenin dize değerini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | `double` örneği; bu örnek nesnenin dize değerini temsil eder. |

