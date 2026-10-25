---
title: "Duration"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir projedeki süreyi temsil eder."
type: docs
weight: 76
url: /tr/java/com.aspose.tasks/duration/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.lang.Struct

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public class Duration extends Struct<Duration> implements System.IEquatable<Duration>
```

Bir projedeki süreyi temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Duration()](#Duration--) | Belirtilen TimeSpan değeri ve TimeUnitType ile yeni bir [Duration](../../com.aspose.tasks/duration) yapısı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [Clone()](#Clone--) | Bu örneğin derin bir kopyasını oluşturur ve döndürür. |
| [CloneTo(Duration that)](#CloneTo-com.aspose.tasks.Duration-) | Örneğin derin bir kopyasını başka bir örneğe yapar. |
| [add(Duration d)](#add-com.aspose.tasks.Duration-) | Belirtilen süreyi bu süreye ekler. |
| [add(double val)](#add-double-) | Belirtilen çift değeri bu süreye ekler. |
| [clone()](#clone--) | \{@inheritDoc\} |
| [convert(byte timeUnitType)](#convert-byte-) | Duration nesnesini belirtilen zaman birimleriyle başka bir süreye dönüştürür. |
| [equals(Duration other)](#equals-com.aspose.tasks.Duration-) | Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür. |
| [equals(Duration obj1, Duration obj2)](#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Belirtilen `obj1` örneğinin belirtilen `obj2` örneğiyle eşit olup olmadığını gösteren bir değer döndürür. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür. |
| [getTimeSpan()](#getTimeSpan--) | Bu Duration nesnesinin `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) örneğini alır. |
| [getTimeUnit()](#getTimeUnit--) | Bu nesne için zaman birimi tipini alır. |
| [hashCode()](#hashCode--) | Bu nesne için bir karma kod değeri döndürür. |
| [isElapsed()](#isElapsed--) | Zaman biriminin geçmiş olup olmadığını gösteren bir değeri alır. |
| [isEstimated()](#isEstimated--) | Zaman biriminin tahmini olup olmadığını gösteren bir değeri alır. |
| [op_Equality(Duration a, Duration b)](#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür. |
| [op_Inequality(Duration a, Duration b)](#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-) | Bu örneğin belirtilen nesneye eşit olmama durumunu belirten bir değeri döndürür. |
| [parse(Project p, String value)](#parse-com.aspose.tasks.Project-java.lang.String-) | Belirtilen dizeyi [Duration](../../com.aspose.tasks/duration) yapısının örneğine dönüştürür. |
| [parseTimeSpan(String value)](#parseTimeSpan-java.lang.String-) | "PT--H--M--S--" biçimindeki süre dizesini ayrıştırır. |
| [subtract(Duration d)](#subtract-com.aspose.tasks.Duration-) | Belirtilen süreyi bu süre örneğinden çıkarır. |
| [subtract(double val)](#subtract-double-) | Belirtilen çift (double) değeri bu süre örneğinden çıkarır. |
| [toDouble()](#toDouble--) | Duration nesnesini `double` değerine dönüştürür. |
| [toString()](#toString--) | Bu örneğin dize temsilini döndürür. |
### Duration() {#Duration--}
```
public Duration()
```


Belirtilen TimeSpan değeri ve TimeUnitType ile yeni bir [Duration](../../com.aspose.tasks/duration) yapısı örneği başlatır.

### Clone() {#Clone--}
```
public Duration Clone()
```


Bu örneğin derin bir kopyasını oluşturur ve döndürür.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a deep copy of this object.
### CloneTo(Duration that) {#CloneTo-com.aspose.tasks.Duration-}
```
public void CloneTo(Duration that)
```


Örneğin derin bir kopyasını başka bir örneğe yapar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| that | [Duration](../../com.aspose.tasks/duration) | başka bir örnek. |

### add(Duration d) {#add-com.aspose.tasks.Duration-}
```
public final Duration add(Duration d)
```


Belirtilen süreyi bu süreye ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | Bu örneğe eklenecek belirtilen [Duration](../../com.aspose.tasks/duration). |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### add(double val) {#add-double-}
```
public final Duration add(double val)
```


Belirtilen çift değeri bu süreye ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer. | double | Bu örneğe eklenecek belirtilen `double` değeri. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance plus the specified duration value.
### clone() {#clone--}
```
public Object clone()
```




**Returns:**
java.lang.Object - \{@inheritDoc\}
### convert(byte timeUnitType) {#convert-byte-}
```
public final Duration convert(byte timeUnitType)
```


Duration nesnesini belirtilen zaman birimleriyle başka bir süreye dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| timeUnitType | byte | belirtilen zaman birimi tipi. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - returns new duration with the specified unit type.
### equals(Duration other) {#equals-com.aspose.tasks.Duration-}
```
public final boolean equals(Duration other)
```


Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | [Duration](../../com.aspose.tasks/duration) | Bu örnek ile karşılaştırılacak nesne. |

**Returns:**
boolean - Returns **True** if other Duration instance has the same TimeSpan and TimeUnit values as this instance; otherwise, **false**.
### equals(Duration obj1, Duration obj2) {#equals-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean equals(Duration obj1, Duration obj2)
```


Belirtilen `obj1` örneğinin belirtilen `obj2` örneğiyle eşit olup olmadığını gösteren bir değer döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj1 | [Duration](../../com.aspose.tasks/duration) | karşılaştırılacak ilk nesne. |
| obj2 | [Duration](../../com.aspose.tasks/duration) | karşılaştırılacak ikinci nesne. |

**Returns:**
boolean - belirtilen `obj1` örneği belirtilen `obj2` örneğine eşitse true döndürür; aksi takdirde false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | Bu örnek ile karşılaştırılacak nesne. |

**Returns:**
boolean - **True** if the specified object is a Duration that has the same TimeSpan and TimeUnit values as this instance; otherwise, **false**.
### getTimeSpan() {#getTimeSpan--}
```
public final double getTimeSpan()
```


Bu Duration nesnesinin `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) örneğini alır.

Değer: Bu Duration nesnesinin TimeSpan örneği.

**Returns:**
double - `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) bu Duration nesnesinin örneği.
### getTimeUnit() {#getTimeUnit--}
```
public final byte getTimeUnit()
```


Bu nesne için zaman birimi tipini alır.

Değer: Bu Duration örneğinin zaman birimi tipi.

**Returns:**
byte - bu nesne için zaman birimi tipi.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Bu nesne için bir karma kod değeri döndürür.

**Returns:**
int - bu süre örneği için bir karma kod değeri döndürür.
### isElapsed() {#isElapsed--}
```
public final boolean isElapsed()
```


Zaman biriminin geçmiş olup olmadığını gösteren bir değeri alır.

Değer: Bu Duration örneğinin geçmiş olup olmadığını belirleyen bayrak.

**Returns:**
boolean - zaman biriminin geçmiş olup olmadığını gösteren bir değer.
### isEstimated() {#isEstimated--}
```
public final boolean isEstimated()
```


Zaman biriminin tahmini olup olmadığını gösteren bir değeri alır.

Değer: Bu Duration örneğinin tahmini olup olmadığını belirleyen bayrak.

**Returns:**
boolean - zaman biriminin tahmini olup olmadığını gösteren bir değer.
### op_Equality(Duration a, Duration b) {#op-Equality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Equality(Duration a, Duration b)
```


Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | İlk süre. |
| b | [Duration](../../com.aspose.tasks/duration) | İkinci süre. |

**Returns:**
boolean - bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değer
### op_Inequality(Duration a, Duration b) {#op-Inequality-com.aspose.tasks.Duration-com.aspose.tasks.Duration-}
```
public static boolean op_Inequality(Duration a, Duration b)
```


Bu örneğin belirtilen nesneye eşit olmama durumunu belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [Duration](../../com.aspose.tasks/duration) | İlk süre. |
| b | [Duration](../../com.aspose.tasks/duration) | İkinci süre. |

**Returns:**
boolean - bu örneğin belirtilen nesneye eşit olmama durumunu belirten bir değer
### parse(Project p, String value) {#parse-com.aspose.tasks.Project-java.lang.String-}
```
public static Duration parse(Project p, String value)
```


Belirtilen dizeyi [Duration](../../com.aspose.tasks/duration) yapısının örneğine dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| p | [Project](../../com.aspose.tasks/project) | belirtilen [Project](../../com.aspose.tasks/project) sınıfının süresini dönüştürmek için örnek. |
| değer | java.lang.String | dönüştürmek için belirtilen dize. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Returns the converted instance of [Duration](../../com.aspose.tasks/duration) struct.
### parseTimeSpan(String value) {#parseTimeSpan-java.lang.String-}
```
public static double parseTimeSpan(String value)
```


"PT--H--M--S--" biçimindeki süre dizesini ayrıştırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | ayrıştırmak için belirtilen dize. |

**Returns:**
double - `TimeSpan`([getTimeSpan](../../com.aspose.tasks/duration\#getTimeSpan--)/[setTimeSpan(TimeSpan)](../../com.aspose.tasks/duration\#setTimeSpan-TimeSpan-)) yapısının ayrıştırılmış örneğini döndürür.
### subtract(Duration d) {#subtract-com.aspose.tasks.Duration-}
```
public final Duration subtract(Duration d)
```


Belirtilen süreyi bu süre örneğinden çıkarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| d | [Duration](../../com.aspose.tasks/duration) | bu örnekten çıkarmak için belirtilen [Duration](../../com.aspose.tasks/duration) örneği. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### subtract(double val) {#subtract-double-}
```
public final Duration subtract(double val)
```


Belirtilen çift (double) değeri bu süre örneğinden çıkarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer. | double | bu örnekten çıkarmak için belirtilen `double` değer. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - New duration object that represents the value of this instance minus the specified duration value.
### toDouble() {#toDouble--}
```
public final double toDouble()
```


Duration nesnesini `double` değerine dönüştürür.

**Returns:**
double - Dönüştürülmüş değer.
### toString() {#toString--}
```
public String toString()
```


Bu örneğin dize temsilini döndürür.

**Returns:**
java.lang.String - bu örneğin dize temsili.
