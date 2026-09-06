---
title: "Temel Çizgi"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir kaynağın temel değerlerini temsil eder."
type: docs
weight: 26
url: /tr/java/com.aspose.tasks/baseline/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public class Baseline implements Comparable<Baseline>, System.IEquatable<Baseline>
```

Bir kaynağın temel değerlerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Baseline()](#Baseline--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [compareTo(Baseline other)](#compareTo-com.aspose.tasks.Baseline-) | IComparable arabirimi uygulaması. |
| [equals(Baseline other)](#equals-com.aspose.tasks.Baseline-) | Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür. |
| [getBaselineNumber()](#getBaselineNumber--) | Bir temel çizgi veri kaydının benzersiz numarasını alır. |
| [getBcwp()](#getBcwp--) | Bir kaynağın bir proje için yaptığı işin bugüne kadar tahmini maliyetini alır. |
| [getBcws()](#getBcws--) | Bir kaynak için planlanan işin bütçe maliyetini alır. |
| [getCost()](#getCost--) | Temel çizgi kaydedildiğinde bir kaynağın tahmini maliyetini alır. |
| [getWork()](#getWork--) | Temel çizgi kaydedildiğinde bir kaynağa atanan işi alır. |
| [hashCode()](#hashCode--) | Temel çizgi için bir karma kod değeri döndürür. |
| [op_Equality(Baseline a, Baseline b)](#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür. |
| [op_GreaterThan(Baseline a, Baseline b)](#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Bu örneğin belirtilen nesneden büyük olup olmadığını belirten bir değeri döndürür. |
| [op_GreaterThanOrEqual(Baseline a, Baseline b)](#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Bu örneğin belirtilen nesneden büyük veya ona eşit olup olmadığını belirten bir değeri döndürür. |
| [op_Inequality(Baseline a, Baseline b)](#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Bu örneğin belirtilen nesneye eşit olmama durumunu belirten bir değeri döndürür. |
| [op_LessThan(Baseline a, Baseline b)](#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Bu örneğin belirtilen nesneden küçük olup olmadığını belirten bir değeri döndürür. |
| [op_LessThanOrEqual(Baseline a, Baseline b)](#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-) | Bu örneğin belirtilen nesneden küçük veya ona eşit olup olmadığını belirten bir değeri döndürür. |
| [setBaselineNumber(int value)](#setBaselineNumber-int-) | Bir temel çizgi veri kaydının benzersiz numarasını ayarlar. |
| [setBcwp(double value)](#setBcwp-double-) | Bir kaynağın bir proje için yaptığı işin bugüne kadar tahmini maliyetini ayarlar. |
| [setBcws(double value)](#setBcws-double-) | Bir kaynak için planlanan işin bütçe maliyetini ayarlar. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Temel çizgi kaydedildiğinde bir kaynağın tahmini maliyetini ayarlar. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Temel çizgi kaydedildiğinde bir kaynağa atanan işi ayarlar. |
### Baseline() {#Baseline--}
```
public Baseline()
```


### compareTo(Baseline other) {#compareTo-com.aspose.tasks.Baseline-}
```
public final int compareTo(Baseline other)
```


IComparable arabirimi uygulaması. Bu örneği belirtilen Baseline nesnesiyle karşılaştırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | bu örneğin karşılaştırılacağı belirtilen Baseline nesnesi. |

**Returns:**
int - bu örnek belirtilen nesneden küçükse -1, büyükse 1 döndürür; aksi takdirde 0 döndürür.
### equals(Baseline other) {#equals-com.aspose.tasks.Baseline-}
```
public final boolean equals(Baseline other)
```


Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | [Baseline](../../com.aspose.tasks/baseline) | bu örnekle karşılaştırılacak belirtilen nesne. |

**Returns:**
boolean - bu örnek belirtilen nesneye eşitse true; aksi takdirde false döndürür.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | bu örnekle karşılaştırılacak belirtilen nesne. |

**Returns:**
boolean - bu örnek belirtilen nesneye eşitse true; aksi takdirde false döndürür.
### getBaselineNumber() {#getBaselineNumber--}
```
public final int getBaselineNumber()
```


Bir temel çizgi veri kaydının benzersiz numarasını alır.

**Returns:**
int - bir temel çizgi veri kaydının benzersiz numarası.
### getBcwp() {#getBcwp--}
```
public final double getBcwp()
```


Bir kaynağın bir proje için yaptığı işin bugüne kadar tahmini maliyetini alır.

**Returns:**
double - bir kaynağın bir proje için yaptığı işin bugüne kadar tahmini maliyeti.
### getBcws() {#getBcws--}
```
public final double getBcws()
```


Bir kaynak için planlanan işin bütçe maliyetini alır.

**Returns:**
double - bir kaynak için planlanan işin bütçe maliyeti.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Temel çizgi kaydedildiğinde bir kaynağın tahmini maliyetini alır.

**Returns:**
java.math.BigDecimal - temel çizgi kaydedildiğinde bir kaynağın tahmini maliyeti.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Temel çizgi kaydedildiğinde bir kaynağa atanan işi alır.

Değer: Temel çizgi kaydedildiğinde bir kaynağa atanan iş miktarı.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the work assigned to a resource when the baseline is saved.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Temel çizgi için bir karma kod değeri döndürür.

**Returns:**
int - bu nesne için bir karma kod değeri döndürür.
### op_Equality(Baseline a, Baseline b) {#op-Equality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Equality(Baseline a, Baseline b)
```


Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | İlk temel çizgi. |
| b | [Baseline](../../com.aspose.tasks/baseline) | İkinci temel çizgi. |

**Returns:**
boolean - bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değer
### op_GreaterThan(Baseline a, Baseline b) {#op-GreaterThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThan(Baseline a, Baseline b)
```


Bu örneğin belirtilen nesneden büyük olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | İlk temel çizgi. |
| b | [Baseline](../../com.aspose.tasks/baseline) | İkinci temel çizgi. |

**Returns:**
boolean - bu örneğin belirtilen nesneden büyük olup olmadığını belirten bir değer
### op_GreaterThanOrEqual(Baseline a, Baseline b) {#op-GreaterThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_GreaterThanOrEqual(Baseline a, Baseline b)
```


Bu örneğin belirtilen nesneden büyük veya ona eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | İlk temel çizgi. |
| b | [Baseline](../../com.aspose.tasks/baseline) | İkinci temel çizgi. |

**Returns:**
boolean - bu örneğin belirtilen nesneden büyük ya da ona eşit olup olmadığını belirten bir değer
### op_Inequality(Baseline a, Baseline b) {#op-Inequality-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_Inequality(Baseline a, Baseline b)
```


Bu örneğin belirtilen nesneye eşit olmama durumunu belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | İlk temel çizgi. |
| b | [Baseline](../../com.aspose.tasks/baseline) | İkinci temel çizgi. |

**Returns:**
boolean - bu örneğin belirtilen nesneye eşit olmama durumunu belirten bir değer
### op_LessThan(Baseline a, Baseline b) {#op-LessThan-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThan(Baseline a, Baseline b)
```


Bu örneğin belirtilen nesneden küçük olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | İlk temel çizgi. |
| b | [Baseline](../../com.aspose.tasks/baseline) | İkinci temel çizgi. |

**Returns:**
boolean - bu örneğin belirtilen nesneden küçük olup olmadığını belirten bir değer
### op_LessThanOrEqual(Baseline a, Baseline b) {#op-LessThanOrEqual-com.aspose.tasks.Baseline-com.aspose.tasks.Baseline-}
```
public static boolean op_LessThanOrEqual(Baseline a, Baseline b)
```


Bu örneğin belirtilen nesneden küçük veya ona eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [Baseline](../../com.aspose.tasks/baseline) | İlk temel çizgi. |
| b | [Baseline](../../com.aspose.tasks/baseline) | İkinci temel çizgi. |

**Returns:**
boolean - bu örneğin belirtilen nesneden küçük ya da ona eşit olup olmadığını belirten bir değer
### setBaselineNumber(int value) {#setBaselineNumber-int-}
```
public final void setBaselineNumber(int value)
```


Bir temel çizgi veri kaydının benzersiz numarasını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | temel çizgi veri kaydının benzersiz numarası. |

### setBcwp(double value) {#setBcwp-double-}
```
public final void setBcwp(double value)
```


Bir kaynağın bir proje için yaptığı işin bugüne kadar tahmini maliyetini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | bir kaynağın bir proje için yaptığı işin bugüne kadar tahmini maliyeti. |

### setBcws(double value) {#setBcws-double-}
```
public final void setBcws(double value)
```


Bir kaynak için planlanan işin bütçe maliyetini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | bir kaynak için planlanan işin bütçe maliyeti. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Temel çizgi kaydedildiğinde bir kaynağın tahmini maliyetini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | temel çizgi kaydedildiğinde bir kaynağın tahmini maliyeti. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Temel çizgi kaydedildiğinde bir kaynağa atanan işi ayarlar.

Değer: Temel çizgi kaydedildiğinde bir kaynağa atanan iş miktarı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | temel çizgi kaydedildiğinde bir kaynağa atanan iş. |

