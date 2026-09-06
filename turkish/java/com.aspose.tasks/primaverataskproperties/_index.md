---
title: "PrimaveraTaskProperties"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Primavera dosyaları XER veya P6XML'den okunan bir görevin Primavera'ye özgü özelliklerini temsil eder."
type: docs
weight: 209
url: /tr/java/com.aspose.tasks/primaverataskproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraTaskProperties
```

Primavera dosyalarından (XER veya P6XML) okunan bir görev için Primavera'ya özgü özellikleri temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getActivityId()](#getActivityId--) | Primavera tarafından kullanılan bir görevin benzersiz tanımlayıcısı olan etkinlik kimliği alanını alır. |
| [getActivityType()](#getActivityType--) | 'Activity Type' alanının değerini alır. |
| [getActualExpenseCost()](#getActualExpenseCost--) | Gerçek harcama maliyetinin değerini alır. |
| [getActualLaborCost()](#getActualLaborCost--) | Gerçek işçilik maliyetinin değerini alır . |
| [getActualLaborUnits()](#getActualLaborUnits--) | Gerçek işçilik birimlerinin değerini alır. |
| [getActualMaterialCost()](#getActualMaterialCost--) | Gerçek malzeme maliyetinin değerini alır. |
| [getActualNonLaborUnits()](#getActualNonLaborUnits--) | Gerçek işçi dışı birimlerin değerini alır. |
| [getActualNonlaborCost()](#getActualNonlaborCost--) | Gerçek işçi dışı maliyetin değerini alır . |
| [getActualTotalCost()](#getActualTotalCost--) | Gerçek maliyetlerin toplam değerini alır. |
| [getBudgetedExpenseCost()](#getBudgetedExpenseCost--) | Bütçelenen (veya planlanan) harcama maliyetinin değerini alır. |
| [getBudgetedLaborCost()](#getBudgetedLaborCost--) | Bütçelenen (veya planlanan) işçilik maliyetinin değerini alır . |
| [getBudgetedMaterialCost()](#getBudgetedMaterialCost--) | Bütçelenen (veya planlanan) malzeme maliyetinin değerini alır. |
| [getBudgetedNonlaborCost()](#getBudgetedNonlaborCost--) | Bütçelenen (veya planlanan) işçi dışı maliyetin değerini alır . |
| [getBudgetedTotalCost()](#getBudgetedTotalCost--) | Bütçelenen (veya planlanan) maliyetlerin toplam değerini alır. |
| [getDurationPercentComplete()](#getDurationPercentComplete--) | Süre yüzde tamamlanma değerini alır. |
| [getDurationType()](#getDurationType--) | Etkinliğin 'Duration Type' alanının değerini alır. |
| [getPercentCompleteType()](#getPercentCompleteType--) | Etkinliğin '% Complete Type' alanının değerini alır. |
| [getPhysicalPercentComplete()](#getPhysicalPercentComplete--) | Fiziksel Yüzde Tamamlanma değerini alır. |
| [getPlannedDuration()](#getPlannedDuration--) | Orijinal veya planlanan süreyi alır -- görevin planlanan başlangıç tarihinden planlanan bitiş tarihine kadar toplam çalışma süresi.. |
| [getPrimaryConstraintDate()](#getPrimaryConstraintDate--) | Birincil kısıtlamanın tarihini alır. |
| [getPrimaryConstraintType()](#getPrimaryConstraintType--) | Birincil kısıtlamanın türünü alır. |
| [getRawActivityType()](#getRawActivityType--) | Etkinliğin 'Activity Type' alanının ham metin temsilini (kaynak dosyada olduğu gibi) alır. |
| [getRawCompletePercentType()](#getRawCompletePercentType--) | Etkinliğin '% Complete Type' alanının ham metin temsilini (kaynak dosyada olduğu gibi) alır. |
| [getRawDurationType()](#getRawDurationType--) | Etkinliğin 'Duration Type' alanının ham metin temsilini (kaynak dosyada olduğu gibi) alır. |
| [getRawStatus()](#getRawStatus--) | Etkinliğin 'Status' alanının ham metin temsilini (kaynak dosyada olduğu gibi) alır. |
| [getRemainingEarlyFinish()](#getRemainingEarlyFinish--) | Kalan erken bitiş tarihini alır - etkinlik için kalan işin tamamlanması planlanan tarih. |
| [getRemainingEarlyStart()](#getRemainingEarlyStart--) | Kalan erken başlangıç tarihini alır - etkinlik için kalan işin başlaması planlanan tarih. |
| [getRemainingExpenseCost()](#getRemainingExpenseCost--) | Kalan harcama maliyetinin değerini alır. |
| [getRemainingLaborUnits()](#getRemainingLaborUnits--) | Kalan iş gücü birimlerinin değerini alır. |
| [getRemainingLateFinish()](#getRemainingLateFinish--) | Kalan geç bitiş tarihini alır. |
| [getRemainingLateStart()](#getRemainingLateStart--) | Kalan geç başlangıç tarihini alır. |
| [getRemainingNonLaborUnits()](#getRemainingNonLaborUnits--) | Kalan iş gücü dışı birimlerin değerini alır. |
| [getSecondaryConstraintDate()](#getSecondaryConstraintDate--) | İkincil kısıtlama tarihini alır. |
| [getSecondaryConstraintType()](#getSecondaryConstraintType--) | İkincil kısıtlama türünü alır. |
| [getSequenceNumber()](#getSequenceNumber--) | WBS öğesinin (özet görevler) sıra numarasını alır. |
| [getUnitsPercentComplete()](#getUnitsPercentComplete--) | Birimlerin yüzde tamamlanma değerini alır. |
### getActivityId() {#getActivityId--}
```
public final String getActivityId()
```


Primavera tarafından kullanılan bir görevin benzersiz tanımlayıcısı olan etkinlik kimliği alanını alır.

--------------------

Yalnızca aktivitelere (özet olmayan görevler) uygulanır.

**Returns:**
java.lang.String - bir aktivite kimliği alanı - Primavera tarafından kullanılan bir görevin benzersiz tanımlayıcısı.
### getActivityType() {#getActivityType--}
```
public final int getActivityType()
```


'Activity Type' alanının değerini alır.

--------------------

Yalnızca aktivitelere (özet olmayan görevler) uygulanır.

**Returns:**
int - 'Activity Type' alanının değeri.
### getActualExpenseCost() {#getActualExpenseCost--}
```
public final BigDecimal getActualExpenseCost()
```


Gerçek harcama maliyetinin değerini alır.

**Returns:**
java.math.BigDecimal - gerçek harcama maliyetinin değeri.
### getActualLaborCost() {#getActualLaborCost--}
```
public final BigDecimal getActualLaborCost()
```


Gerçek işçilik maliyetinin değerini alır .

**Returns:**
java.math.BigDecimal - gerçek iş gücü maliyetinin değeri.
### getActualLaborUnits() {#getActualLaborUnits--}
```
public final double getActualLaborUnits()
```


Gerçek işçilik birimlerinin değerini alır.

**Returns:**
double - gerçek iş gücü birimlerinin değeri.
### getActualMaterialCost() {#getActualMaterialCost--}
```
public final BigDecimal getActualMaterialCost()
```


Gerçek malzeme maliyetinin değerini alır.

**Returns:**
java.math.BigDecimal - gerçek malzeme maliyetinin değeri.
### getActualNonLaborUnits() {#getActualNonLaborUnits--}
```
public final double getActualNonLaborUnits()
```


Gerçek işçi dışı birimlerin değerini alır.

**Returns:**
double - gerçek iş gücü dışı birimlerin değeri.
### getActualNonlaborCost() {#getActualNonlaborCost--}
```
public final BigDecimal getActualNonlaborCost()
```


Gerçek işçi dışı maliyetin değerini alır .

**Returns:**
java.math.BigDecimal - gerçek iş gücü dışı maliyetin değeri.
### getActualTotalCost() {#getActualTotalCost--}
```
public final BigDecimal getActualTotalCost()
```


Gerçek maliyetlerin toplam değerini alır.

**Returns:**
java.math.BigDecimal - gerçek maliyetlerin toplam değeri.
### getBudgetedExpenseCost() {#getBudgetedExpenseCost--}
```
public final BigDecimal getBudgetedExpenseCost()
```


Bütçelenen (veya planlanan) harcama maliyetinin değerini alır.

**Returns:**
java.math.BigDecimal - bütçelenen (veya planlanan) harcama maliyetinin değeri.
### getBudgetedLaborCost() {#getBudgetedLaborCost--}
```
public final BigDecimal getBudgetedLaborCost()
```


Bütçelenen (veya planlanan) işçilik maliyetinin değerini alır .

**Returns:**
java.math.BigDecimal - bütçelenen (veya planlanan) iş gücü maliyetinin değeri.
### getBudgetedMaterialCost() {#getBudgetedMaterialCost--}
```
public final BigDecimal getBudgetedMaterialCost()
```


Bütçelenen (veya planlanan) malzeme maliyetinin değerini alır.

**Returns:**
java.math.BigDecimal - bütçelenen (veya planlanan) malzeme maliyetinin değeri.
### getBudgetedNonlaborCost() {#getBudgetedNonlaborCost--}
```
public final BigDecimal getBudgetedNonlaborCost()
```


Bütçelenen (veya planlanan) işçi dışı maliyetin değerini alır .

**Returns:**
java.math.BigDecimal - bütçelenen (veya planlanan) iş gücü dışı maliyetin değeri.
### getBudgetedTotalCost() {#getBudgetedTotalCost--}
```
public final BigDecimal getBudgetedTotalCost()
```


Bütçelenen (veya planlanan) maliyetlerin toplam değerini alır.

**Returns:**
java.math.BigDecimal - bütçelenen (veya planlanan) maliyetlerin toplam değeri.
### getDurationPercentComplete() {#getDurationPercentComplete--}
```
public final double getDurationPercentComplete()
```


Süre yüzde tamamlanma değerini alır.

**Returns:**
double - sürenin yüzde tamamlanma değeri.
### getDurationType() {#getDurationType--}
```
public final int getDurationType()
```


Etkinliğin 'Duration Type' alanının değerini alır.

--------------------

Yalnızca aktivitelere (özet olmayan görevler) uygulanır.

**Returns:**
int - aktivitenin 'Duration Type' alanının değeri.
### getPercentCompleteType() {#getPercentCompleteType--}
```
public final int getPercentCompleteType()
```


Etkinliğin '% Complete Type' alanının değerini alır.

--------------------

Yalnızca aktivitelere (özet olmayan görevler) uygulanır.

**Returns:**
int - etkinliğin '% Complete Type' alanının değeri.
### getPhysicalPercentComplete() {#getPhysicalPercentComplete--}
```
public final double getPhysicalPercentComplete()
```


Fiziksel Yüzde Tamamlanma değerini alır.

--------------------

Yalnızca aktivitelere (özet olmayan görevler) uygulanır.

**Returns:**
double - Physical Percent Complete değerinin değeri.
### getPlannedDuration() {#getPlannedDuration--}
```
public final Duration getPlannedDuration()
```


Orijinal veya planlanan süreyi alır -- görevin planlanan başlangıç tarihinden planlanan bitiş tarihine kadar toplam çalışma süresi..

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the original or planned duration -- the total working time from the task planned start date to the planned finish date.
### getPrimaryConstraintDate() {#getPrimaryConstraintDate--}
```
public final Date getPrimaryConstraintDate()
```


Birincil kısıtlamanın tarihini alır.

**Returns:**
java.util.Date - birincil kısıtlamanın tarihi.
### getPrimaryConstraintType() {#getPrimaryConstraintType--}
```
public final int getPrimaryConstraintType()
```


Birincil kısıtlamanın türünü alır.

**Returns:**
int - birincil kısıtlamanın türü.
### getRawActivityType() {#getRawActivityType--}
```
public final String getRawActivityType()
```


Etkinliğin 'Activity Type' alanının ham metin temsilini (kaynak dosyada olduğu gibi) alır.

--------------------

Yalnızca aktivitelere (özet olmayan görevler) uygulanır.

**Returns:**
java.lang.String - etkinliğin 'Activity Type' alanının ham metin temsili (kaynak dosyada olduğu gibi).
### getRawCompletePercentType() {#getRawCompletePercentType--}
```
public final String getRawCompletePercentType()
```


Etkinliğin '% Complete Type' alanının ham metin temsilini (kaynak dosyada olduğu gibi) alır.

--------------------

Yalnızca aktivitelere (özet olmayan görevler) uygulanır.

**Returns:**
java.lang.String - etkinliğin '% Complete Type' alanının ham metin temsili (kaynak dosyada olduğu gibi).
### getRawDurationType() {#getRawDurationType--}
```
public final String getRawDurationType()
```


Etkinliğin 'Duration Type' alanının ham metin temsilini (kaynak dosyada olduğu gibi) alır.

--------------------

Yalnızca aktivitelere (özet olmayan görevler) uygulanır.

**Returns:**
java.lang.String - etkinliğin 'Duration Type' alanının ham metin temsili (kaynak dosyada olduğu gibi).
### getRawStatus() {#getRawStatus--}
```
public final String getRawStatus()
```


Etkinliğin 'Status' alanının ham metin temsilini (kaynak dosyada olduğu gibi) alır.

--------------------

Yalnızca aktivitelere (özet olmayan görevler) uygulanır.

**Returns:**
java.lang.String - etkinliğin 'Status' alanının ham metin temsili (kaynak dosyada olduğu gibi).
### getRemainingEarlyFinish() {#getRemainingEarlyFinish--}
```
public final Date getRemainingEarlyFinish()
```


Kalan erken bitiş tarihini alır - etkinlik için kalan işin tamamlanması planlanan tarih.

**Returns:**
java.util.Date - kalan erken bitiş tarihi - etkinlik için kalan işin tamamlanması planlanan tarih.
### getRemainingEarlyStart() {#getRemainingEarlyStart--}
```
public final Date getRemainingEarlyStart()
```


Kalan erken başlangıç tarihini alır - etkinlik için kalan işin başlaması planlanan tarih.

**Returns:**
java.util.Date - kalan erken başlangıç tarihi - etkinlik için kalan işin başlaması planlanan tarih.
### getRemainingExpenseCost() {#getRemainingExpenseCost--}
```
public final BigDecimal getRemainingExpenseCost()
```


Kalan harcama maliyetinin değerini alır.

**Returns:**
java.math.BigDecimal - kalan gider maliyetinin değeri.
### getRemainingLaborUnits() {#getRemainingLaborUnits--}
```
public final double getRemainingLaborUnits()
```


Kalan iş gücü birimlerinin değerini alır.

**Returns:**
double - kalan iş gücü birimlerinin değeri.
### getRemainingLateFinish() {#getRemainingLateFinish--}
```
public final Date getRemainingLateFinish()
```


Kalan geç bitiş tarihini alır.

**Returns:**
java.util.Date - kalan geç bitiş tarihi.
### getRemainingLateStart() {#getRemainingLateStart--}
```
public final Date getRemainingLateStart()
```


Kalan geç başlangıç tarihini alır.

**Returns:**
java.util.Date - kalan geç başlangıç tarihi.
### getRemainingNonLaborUnits() {#getRemainingNonLaborUnits--}
```
public final double getRemainingNonLaborUnits()
```


Kalan iş gücü dışı birimlerin değerini alır.

**Returns:**
double - kalan iş gücü dışı birimlerin değeri.
### getSecondaryConstraintDate() {#getSecondaryConstraintDate--}
```
public final Date getSecondaryConstraintDate()
```


İkincil kısıtlama tarihini alır.

**Returns:**
java.util.Date - ikincil kısıtlamanın tarihi.
### getSecondaryConstraintType() {#getSecondaryConstraintType--}
```
public final int getSecondaryConstraintType()
```


İkincil kısıtlama türünü alır.

**Returns:**
int - ikincil kısıtlamanın türü.
### getSequenceNumber() {#getSequenceNumber--}
```
public final int getSequenceNumber()
```


WBS öğesinin (özet görevler) sıra numarasını alır. Primavera'da özet görevleri sıralamak için kullanılır.

--------------------

WBS öğelerine (özet görevler) uygulanır.

**Returns:**
int - WBS öğesinin (özet görevler) sıra numarası.
### getUnitsPercentComplete() {#getUnitsPercentComplete--}
```
public final double getUnitsPercentComplete()
```


Birimlerin yüzde tamamlanma değerini alır.

**Returns:**
double - birimlerin yüzde tamamlanma değerinin değeri.
