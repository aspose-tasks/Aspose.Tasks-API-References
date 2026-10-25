---
title: "RiskPattern"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir proje görevi için risk desenini temsil eder."
type: docs
weight: 268
url: /tr/java/com.aspose.tasks/riskpattern/
---

**Inheritance:**
java.lang.Object
```
public class RiskPattern
```

Bir proje görevi için risk desenini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [RiskPattern(Task task)](#RiskPattern-com.aspose.tasks.Task-) | Yeni bir [RiskPattern](../../com.aspose.tasks/riskpattern) sınıf örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getConfidenceLevel()](#getConfidenceLevel--) | Gerçek üretilen değerlerin iyimser ve kötümser tahminler içinde olacağı zaman yüzdesine karşılık gelen güven düzeyini alır. |
| [getDistribution()](#getDistribution--) | Monte Carlo simülasyonunda kullanılan olasılık dağılımını alır. |
| [getOptimistic()](#getOptimistic--) | En iyi olası proje senaryosunda gerçekleşebilecek en muhtemel görev süresinin yüzdesini alır. |
| [getPessimistic()](#getPessimistic--) | En kötü olası proje senaryosunda gerçekleşebilecek en muhtemel görev süresinin yüzdesini alır. |
| [getTask()](#getTask--) | Bu risk deseninin uygulandığı bir proje görevini alır. |
| [setConfidenceLevel(int value)](#setConfidenceLevel-int-) | Gerçek oluşturulan değerlerin iyimser ve kötümser tahminler içinde olacağı zaman yüzdesine karşılık gelen güven düzeyini ayarlar. |
| [setDistribution(int value)](#setDistribution-int-) | Monte Carlo simülasyonunda kullanılan olasılık dağılımını ayarlar. |
| [setOptimistic(int value)](#setOptimistic-int-) | En iyi olası proje senaryosunda gerçekleşebilecek en muhtemel görev süresinin yüzdesini ayarlar. |
| [setPessimistic(int value)](#setPessimistic-int-) | En kötü olası proje senaryosunda gerçekleşebilecek en muhtemel görev süresinin yüzdesini ayarlar. |
### RiskPattern(Task task) {#RiskPattern-com.aspose.tasks.Task-}
```
public RiskPattern(Task task)
```


Yeni bir [RiskPattern](../../com.aspose.tasks/riskpattern) sınıf örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Monte Carlo simülasyonunda bu riskin uygulanacağı belirtilen proje görevi. |

### getConfidenceLevel() {#getConfidenceLevel--}
```
public final int getConfidenceLevel()
```


Gerçek oluşturulan değerlerin iyimser ve kötümser tahminler içinde olacağı zaman yüzdesine karşılık gelen güven düzeyini alır. Varsayılan değer CL99'dur.

--------------------

`ConfidenceLevel`([getConfidenceLevel()](../../com.aspose/tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose/tasks/riskpattern\#setConfidenceLevel-int-)) enum'unda tanımlanan değerlerden biri olabilir.

**Returns:**
int - gerçek oluşturulan değerlerin iyimser ve kötümser tahminler içinde olacağı zaman yüzdesine karşılık gelen güven düzeyi.
### getDistribution() {#getDistribution--}
```
public final int getDistribution()
```


Monte Carlo simülasyonunda kullanılan olasılık dağılımını alır. Varsayılan değer ProbabilityDistributionType.Normal'dur.

--------------------

[ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype) enum'unda tanımlanan değerlerden biri olabilir.

**Returns:**
int - Monte Carlo simülasyonunda kullanılan olasılık dağılımı.
### getOptimistic() {#getOptimistic--}
```
public final int getOptimistic()
```


En iyi olası proje senaryosunda gerçekleşebilecek en muhtemel görev süresinin yüzdesini alır. Varsayılan değer 75'tir, bu da tahmini belirtilen görev süresi 4 gün ise iyimser sürenin 3 gün olacağı anlamına gelir.

**Returns:**
int - En iyi olası proje senaryosunda gerçekleşebilecek en muhtemel görev süresinin yüzdesi.
### getPessimistic() {#getPessimistic--}
```
public final int getPessimistic()
```


En kötü olası proje senaryosunda gerçekleşebilecek en muhtemel görev süresinin yüzdesini alır. Varsayılan değer 125'tir, bu da tahmini belirtilen görev süresi 4 gün ise kötümser sürenin 5 gün olacağı anlamına gelir.

**Returns:**
int - En kötü olası proje senaryosunda gerçekleşebilecek en muhtemel görev süresinin yüzdesi.
### getTask() {#getTask--}
```
public final Task getTask()
```


Bu risk deseninin uygulandığı bir proje görevini alır.

**Returns:**
[Task](../../com.aspose.tasks/task) - a project task to which this risk pattern is applied.
### setConfidenceLevel(int value) {#setConfidenceLevel-int-}
```
public final void setConfidenceLevel(int value)
```


Gerçek oluşturulan değerlerin iyimser ve kötümser tahminler içinde olacağı zaman yüzdesine karşılık gelen güven düzeyini ayarlar. Varsayılan değer CL99'dur.

--------------------

`ConfidenceLevel`([getConfidenceLevel()](../../com.aspose/tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose/tasks/riskpattern\#setConfidenceLevel-int-)) enum'unda tanımlanan değerlerden biri olabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | gerçek oluşturulan değerlerin iyimser ve kötümser tahminler içinde olacağı zaman yüzdesine karşılık gelen güven düzeyi. |

### setDistribution(int value) {#setDistribution-int-}
```
public final void setDistribution(int value)
```


Monte Carlo simülasyonunda kullanılan olasılık dağılımını ayarlar. Varsayılan değer ProbabilityDistributionType.Normal'dur.

--------------------

[ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype) enum'unda tanımlanan değerlerden biri olabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Monte Carlo simülasyonunda kullanılan olasılık dağılımı. |

### setOptimistic(int value) {#setOptimistic-int-}
```
public final void setOptimistic(int value)
```


En iyi olası proje senaryosunda gerçekleşebilecek en muhtemel görev süresinin yüzdesini ayarlar. Varsayılan değer 75'tir, bu da tahmini belirtilen görev süresi 4 gün ise iyimser sürenin 3 gün olacağı anlamına gelir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | En iyi olası proje senaryosunda gerçekleşebilecek en muhtemel görev süresinin yüzdesi. |

### setPessimistic(int value) {#setPessimistic-int-}
```
public final void setPessimistic(int value)
```


En kötü olası proje senaryosunda gerçekleşebilecek en muhtemel görev süresinin yüzdesini ayarlar. Varsayılan değer 125'tir, bu da tahmini belirtilen görev süresi 4 gün ise kötümser sürenin 5 gün olacağı anlamına gelir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | En kötü olası proje senaryosunda gerçekleşebilecek en muhtemel görev süresinin yüzdesi. |

