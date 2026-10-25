---
title: "Oran"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir zaman diliminin ve bu süre içinde bir kaynak için geçerli olan oranların tanımını temsil eder."
type: docs
weight: 232
url: /tr/java/com.aspose.tasks/rate/
---

**Inheritance:**
java.lang.Object
```
public class Rate
```

Bir zaman diliminin ve bu süre içinde bir kaynak için geçerli olan oranların tanımını temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCostPerUse()](#getCostPerUse--) | Bir kaynağın kullanım başına maliyetini alır. |
| [getOvertimeRate()](#getOvertimeRate--) | Bir kaynak için saat başına fazla mesai oranını alır. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Microsoft Project'in fazla mesai oranını göstermek için kullandığı birimleri alır. |
| [getRateTable()](#getRateTable--) | Bir kaynak için oran tablosunun benzersiz tanımlayıcısını alır. |
| [getRatesFrom()](#getRatesFrom--) | Bir oranının yürürlüğe girdiği tarihi alır. |
| [getRatesTo()](#getRatesTo--) | Bir oranının geçerli olduğu son tarihi alır. |
| [getStandardRate()](#getStandardRate--) | Bir kaynak için saat başına standart oranı alır. |
| [getStandardRateFormat()](#getStandardRateFormat--) | Microsoft Project'in standart oranı göstermek için kullandığı birimleri alır. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | Bir kaynağın kullanım başına maliyetini ayarlar. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | Bir kaynak için saat başına fazla mesai oranını ayarlar. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Microsoft Project'in fazla mesai oranını görüntülemek için kullandığı birimleri ayarlar. |
| [setRateTable(int value)](#setRateTable-int-) | Bir kaynak için oran tablosunun benzersiz tanımlayıcısını ayarlar. |
| [setRatesFrom(Date value)](#setRatesFrom-java.util.Date-) | Bir oranının yürürlüğe girdiği tarihi ayarlar. |
| [setRatesTo(Date value)](#setRatesTo-java.util.Date-) | Bir oranının geçerli olduğu son tarihi ayarlar. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | Bir kaynak için saat başına standart oranı ayarlar. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Microsoft Project'in standart oranı görüntülemek için kullandığı birimleri ayarlar. |
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


Bir kaynağın kullanım başına maliyetini alır. Bu değer, kaynak için bir oran tablosu mevcutsa geçerli tarihten alınır.

**Returns:**
java.math.BigDecimal - bir kaynağın kullanım başına maliyeti.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


Bir kaynak için saat başına fazla mesai oranını alır.

**Returns:**
java.math.BigDecimal - bir kaynak için saat başına fazla mesai oranı.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Microsoft Project'in fazla mesai oranını göstermek için kullandığı birimleri alır.

**Returns:**
int - Microsoft Project'in fazla mesai oranını görüntülemek için kullandığı birimler.
### getRateTable() {#getRateTable--}
```
public final int getRateTable()
```


Bir kaynak için oran tablosunun benzersiz tanımlayıcısını alır.

**Returns:**
int - bir kaynak için oran tablosunun benzersiz tanımlayıcısı.
### getRatesFrom() {#getRatesFrom--}
```
public final Date getRatesFrom()
```


Bir oranının yürürlüğe girdiği tarihi alır.

**Returns:**
java.util.Date - bir oranının yürürlüğe girdiği tarih.
### getRatesTo() {#getRatesTo--}
```
public final Date getRatesTo()
```


Bir oranının geçerli olduğu son tarihi alır.

**Returns:**
java.util.Date - bir oranının geçerli olduğu son tarih.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


Bir kaynak için saat başına standart oranı alır.

**Returns:**
java.math.BigDecimal - bir kaynak için saat başına standart oran.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Microsoft Project'in standart oranı göstermek için kullandığı birimleri alır.

**Returns:**
int - Microsoft Project'in standart oranı görüntülemek için kullandığı birimler.
### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


Bir kaynağın kullanım başına maliyetini ayarlar. Bu değer, kaynak için bir oran tablosu mevcutsa geçerli tarihten alınır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | kaynağın kullanım başına maliyeti. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


Bir kaynak için saat başına fazla mesai oranını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | kaynak için saat başına fazla mesai oranı. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Microsoft Project'in fazla mesai oranını görüntülemek için kullandığı birimleri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Microsoft Project'in fazla mesai oranını görüntülemek için kullandığı birimler. |

### setRateTable(int value) {#setRateTable-int-}
```
public final void setRateTable(int value)
```


Bir kaynak için oran tablosunun benzersiz tanımlayıcısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | bir kaynak için oran tablosunun benzersiz tanımlayıcısı. |

### setRatesFrom(Date value) {#setRatesFrom-java.util.Date-}
```
public final void setRatesFrom(Date value)
```


Bir oranının yürürlüğe girdiği tarihi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | bir oranının yürürlüğe girdiği tarih. |

### setRatesTo(Date value) {#setRatesTo-java.util.Date-}
```
public final void setRatesTo(Date value)
```


Bir oranının geçerli olduğu son tarihi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | bir oranının geçerli olduğu son tarih. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


Bir kaynak için saat başına standart oranı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | bir kaynak için saat başına standart oran. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Microsoft Project'in standart oranı görüntülemek için kullandığı birimleri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Microsoft Project tarafından standart oranı görüntülemek için kullanılan birimler. |

