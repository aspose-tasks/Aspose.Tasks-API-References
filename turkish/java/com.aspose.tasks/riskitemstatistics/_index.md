---
title: "RiskItemStatistics"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Analiz edilen projenin görevi için istatistiksel verileri depolayan bir öğeyi temsil eder."
type: docs
weight: 265
url: /tr/java/com.aspose.tasks/riskitemstatistics/
---

**Inheritance:**
java.lang.Object
```
public class RiskItemStatistics
```

Analiz edilen projenin görevi için istatistiksel verileri depolayan bir öğeyi temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getExpectedValue()](#getExpectedValue--) | Risk öğesinin beklenen değerini alır. |
| [getItemType()](#getItemType--) | [RiskItemType](../../com.aspose.tasks/riskitemtype) enum'ının bir örneğini alır. |
| [getMaximum()](#getMaximum--) | Monte Carlo simülasyonu sırasında üretilen maksimum değeri alır. |
| [getMinimum()](#getMinimum--) | Monte Carlo simülasyonu sırasında üretilen minimum değeri alır. |
| [getPercentile(int percent)](#getPercentile-int-) | Üretilen örneklerin belirli bir yüzdesinin altında kaldığı bir değeri alır. |
| [getStandardDeviation()](#getStandardDeviation--) | Risk öğesinin standart sapmasını alır. |
| [toString()](#toString--) | Risk öğesinin kısa metin temsilini döndürür. |
### getExpectedValue() {#getExpectedValue--}
```
public final Date getExpectedValue()
```


Risk öğesinin beklenen değerini alır.

**Returns:**
java.util.Date - risk öğesinin beklenen değeri.
### getItemType() {#getItemType--}
```
public final int getItemType()
```


[RiskItemType](../../com.aspose.tasks/riskitemtype) enum'ının bir örneğini alır.

**Returns:**
int - [RiskItemType](../../com.aspose.tasks/riskitemtype) enum'ının bir örneği.
### getMaximum() {#getMaximum--}
```
public final Date getMaximum()
```


Monte Carlo simülasyonu sırasında üretilen maksimum değeri alır.

**Returns:**
java.util.Date - Monte Carlo simülasyonu sırasında üretilen maksimum değer.
### getMinimum() {#getMinimum--}
```
public final Date getMinimum()
```


Monte Carlo simülasyonu sırasında üretilen minimum değeri alır.

**Returns:**
java.util.Date - Monte Carlo simülasyonu sırasında üretilen minimum değer.
### getPercentile(int percent) {#getPercentile-int-}
```
public final Date getPercentile(int percent)
```


Üretilen örneklerin belirli bir yüzdesinin altında kaldığı bir değeri alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yüzde | int | 0 ile 100 arasında belirtilen yüzde. |

**Returns:**
java.util.Date - üretilen örneklerin belirtilen bir yüzdesinin altında kalan değer.
### getStandardDeviation() {#getStandardDeviation--}
```
public final Duration getStandardDeviation()
```


Risk öğesinin standart sapmasını alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the standard deviation of the risk item.
### toString() {#toString--}
```
public String toString()
```


Risk öğesinin kısa dize temsilini döndürür. Temsilin kesin ayrıntıları belirtilmemiştir ve değişebilir.

**Returns:**
java.lang.String - RiskItem nesnesini temsil eden kısa dize.
