---
title: "PrimaveraTaskProperties"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar Primavera-specifika egenskaper för en uppgift som läses från Primavera-filer XER eller P6XML."
type: docs
weight: 209
url: /sv/java/com.aspose.tasks/primaverataskproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraTaskProperties
```

Representerar Primavera-specifika egenskaper för en uppgift som lästs från Primavera-filer (XER eller P6XML).
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getActivityId()](#getActivityId--) | Hämtar ett aktivitets‑id‑fält – en uppgifts unika identifierare som används av Primavera. |
| [getActivityType()](#getActivityType--) | Hämtar värdet för fältet 'Activity Type'. |
| [getActualExpenseCost()](#getActualExpenseCost--) | Hämtar värdet för den faktiska utgiftkostnaden. |
| [getActualLaborCost()](#getActualLaborCost--) | Hämtar värdet för den faktiska arbetskostnaden. |
| [getActualLaborUnits()](#getActualLaborUnits--) | Hämtar värdet för faktiska arbetsenheter. |
| [getActualMaterialCost()](#getActualMaterialCost--) | Hämtar värdet för den faktiska materialkostnaden. |
| [getActualNonLaborUnits()](#getActualNonLaborUnits--) | Hämtar värdet för faktiska icke‑arbetsenheter. |
| [getActualNonlaborCost()](#getActualNonlaborCost--) | Hämtar värdet för den faktiska icke‑arbetskostnaden. |
| [getActualTotalCost()](#getActualTotalCost--) | Hämtar det totala värdet för faktiska kostnader. |
| [getBudgetedExpenseCost()](#getBudgetedExpenseCost--) | Hämtar värdet för budgeterad (eller planerad) utgiftkostnad. |
| [getBudgetedLaborCost()](#getBudgetedLaborCost--) | Hämtar värdet för budgeterad (eller planerad) arbetskostnad. |
| [getBudgetedMaterialCost()](#getBudgetedMaterialCost--) | Hämtar värdet för budgeterad (eller planerad) materialkostnad. |
| [getBudgetedNonlaborCost()](#getBudgetedNonlaborCost--) | Hämtar värdet för budgeterad (eller planerad) icke‑arbetskostnad. |
| [getBudgetedTotalCost()](#getBudgetedTotalCost--) | Hämtar det totala värdet för budgeterade (eller planerade) kostnader. |
| [getDurationPercentComplete()](#getDurationPercentComplete--) | Hämtar värdet för varaktighetens färdigställandeprocent. |
| [getDurationType()](#getDurationType--) | Hämtar värdet för fältet 'Duration Type' för aktiviteten. |
| [getPercentCompleteType()](#getPercentCompleteType--) | Hämtar värdet för fältet '% Complete Type' för aktiviteten. |
| [getPhysicalPercentComplete()](#getPhysicalPercentComplete--) | Hämtar värdet för fysisk färdigställandeprocent. |
| [getPlannedDuration()](#getPlannedDuration--) | Hämtar den ursprungliga eller planerade varaktigheten – den totala arbetstiden från uppgiftens planerade startdatum till det planerade slutdatumet. |
| [getPrimaryConstraintDate()](#getPrimaryConstraintDate--) | Hämtar datumet för primär begränsning. |
| [getPrimaryConstraintType()](#getPrimaryConstraintType--) | Hämtar en typ av primär begränsning. |
| [getRawActivityType()](#getRawActivityType--) | Hämtar råtextrepresentation (som i källfilen) av fältet 'Activity Type' för aktiviteten. |
| [getRawCompletePercentType()](#getRawCompletePercentType--) | Hämtar råtextrepresentation (som i källfilen) av fältet '% Complete Type' för aktiviteten. |
| [getRawDurationType()](#getRawDurationType--) | Hämtar råtextrepresentation (som i källfilen) av fältet 'Duration Type' för aktiviteten. |
| [getRawStatus()](#getRawStatus--) | Hämtar råtextrepresentation (som i källfilen) av fältet 'Status' för aktiviteten. |
| [getRemainingEarlyFinish()](#getRemainingEarlyFinish--) | Hämtar återstående tidigt avslutsdatum - datumet då det återstående arbetet för aktiviteten är planerat att avslutas. |
| [getRemainingEarlyStart()](#getRemainingEarlyStart--) | Hämtar återstående tidigt startdatum - datumet då det återstående arbetet för aktiviteten är planerat att påbörjas. |
| [getRemainingExpenseCost()](#getRemainingExpenseCost--) | Hämtar värdet av återstående utgiftkostnad. |
| [getRemainingLaborUnits()](#getRemainingLaborUnits--) | Hämtar värdet av återstående arbetsenheter. |
| [getRemainingLateFinish()](#getRemainingLateFinish--) | Hämtar återstående sent avslutsdatum. |
| [getRemainingLateStart()](#getRemainingLateStart--) | Hämtar återstående sent startdatum. |
| [getRemainingNonLaborUnits()](#getRemainingNonLaborUnits--) | Hämtar värdet av återstående icke‑arbetsenheter. |
| [getSecondaryConstraintDate()](#getSecondaryConstraintDate--) | Hämtar datumet för sekundär begränsning. |
| [getSecondaryConstraintType()](#getSecondaryConstraintType--) | Hämtar en typ av sekundär begränsning. |
| [getSequenceNumber()](#getSequenceNumber--) | Hämtar sekvensnumret för WBS-posten (sammanfattande uppgifter). |
| [getUnitsPercentComplete()](#getUnitsPercentComplete--) | Hämtar värdet av enheternas procentuella slutförande. |
### getActivityId() {#getActivityId--}
```
public final String getActivityId()
```


Hämtar ett aktivitets‑id‑fält – en uppgifts unika identifierare som används av Primavera.

--------------------

Gäller endast för aktiviteter (icke‑sammanfattande uppgifter).

**Returns:**
java.lang.String - ett aktivitets-id-fält - en uppgiftens unika identifierare som används av Primavera.
### getActivityType() {#getActivityType--}
```
public final int getActivityType()
```


Hämtar värdet för fältet 'Activity Type'.

--------------------

Gäller endast för aktiviteter (icke‑sammanfattande uppgifter).

**Returns:**
int - värdet av fältet 'Activity Type'.
### getActualExpenseCost() {#getActualExpenseCost--}
```
public final BigDecimal getActualExpenseCost()
```


Hämtar värdet för den faktiska utgiftkostnaden.

**Returns:**
java.math.BigDecimal - värdet av faktisk utgiftkostnad.
### getActualLaborCost() {#getActualLaborCost--}
```
public final BigDecimal getActualLaborCost()
```


Hämtar värdet för den faktiska arbetskostnaden.

**Returns:**
java.math.BigDecimal - värdet av faktisk arbetskostnad .
### getActualLaborUnits() {#getActualLaborUnits--}
```
public final double getActualLaborUnits()
```


Hämtar värdet för faktiska arbetsenheter.

**Returns:**
double - värdet av faktiska arbetsenheter.
### getActualMaterialCost() {#getActualMaterialCost--}
```
public final BigDecimal getActualMaterialCost()
```


Hämtar värdet för den faktiska materialkostnaden.

**Returns:**
java.math.BigDecimal - värdet av faktisk materialkostnad.
### getActualNonLaborUnits() {#getActualNonLaborUnits--}
```
public final double getActualNonLaborUnits()
```


Hämtar värdet för faktiska icke‑arbetsenheter.

**Returns:**
double - värdet av faktiska icke‑arbetsenheter.
### getActualNonlaborCost() {#getActualNonlaborCost--}
```
public final BigDecimal getActualNonlaborCost()
```


Hämtar värdet för den faktiska icke‑arbetskostnaden.

**Returns:**
java.math.BigDecimal - värdet av faktisk icke‑arbetskostnad .
### getActualTotalCost() {#getActualTotalCost--}
```
public final BigDecimal getActualTotalCost()
```


Hämtar det totala värdet för faktiska kostnader.

**Returns:**
java.math.BigDecimal - det totala värdet av faktiska kostnader.
### getBudgetedExpenseCost() {#getBudgetedExpenseCost--}
```
public final BigDecimal getBudgetedExpenseCost()
```


Hämtar värdet för budgeterad (eller planerad) utgiftkostnad.

**Returns:**
java.math.BigDecimal - värdet av budgeterad (eller planerad) utgift.
### getBudgetedLaborCost() {#getBudgetedLaborCost--}
```
public final BigDecimal getBudgetedLaborCost()
```


Hämtar värdet för budgeterad (eller planerad) arbetskostnad.

**Returns:**
java.math.BigDecimal - värdet av budgeterad (eller planerad) arbetskostnad.
### getBudgetedMaterialCost() {#getBudgetedMaterialCost--}
```
public final BigDecimal getBudgetedMaterialCost()
```


Hämtar värdet för budgeterad (eller planerad) materialkostnad.

**Returns:**
java.math.BigDecimal - värdet av budgeterad (eller planerad) materialkostnad.
### getBudgetedNonlaborCost() {#getBudgetedNonlaborCost--}
```
public final BigDecimal getBudgetedNonlaborCost()
```


Hämtar värdet för budgeterad (eller planerad) icke‑arbetskostnad.

**Returns:**
java.math.BigDecimal - värdet av budgeterad (eller planerad) icke-arbetskostnad.
### getBudgetedTotalCost() {#getBudgetedTotalCost--}
```
public final BigDecimal getBudgetedTotalCost()
```


Hämtar det totala värdet för budgeterade (eller planerade) kostnader.

**Returns:**
java.math.BigDecimal - det totala värdet av budgeterade (eller planerade) kostnader.
### getDurationPercentComplete() {#getDurationPercentComplete--}
```
public final double getDurationPercentComplete()
```


Hämtar värdet för varaktighetens färdigställandeprocent.

**Returns:**
double - värdet av varaktighetens färdigställda procent.
### getDurationType() {#getDurationType--}
```
public final int getDurationType()
```


Hämtar värdet för fältet 'Duration Type' för aktiviteten.

--------------------

Gäller endast för aktiviteter (icke‑sammanfattande uppgifter).

**Returns:**
int - värdet av fältet 'Duration Type' för aktiviteten.
### getPercentCompleteType() {#getPercentCompleteType--}
```
public final int getPercentCompleteType()
```


Hämtar värdet för fältet '% Complete Type' för aktiviteten.

--------------------

Gäller endast för aktiviteter (icke‑sammanfattande uppgifter).

**Returns:**
int - värdet av fältet '% Complete Type' för aktiviteten.
### getPhysicalPercentComplete() {#getPhysicalPercentComplete--}
```
public final double getPhysicalPercentComplete()
```


Hämtar värdet för fysisk färdigställandeprocent.

--------------------

Gäller endast för aktiviteter (icke‑sammanfattande uppgifter).

**Returns:**
double - värdet av fysisk procentuell färdigställning.
### getPlannedDuration() {#getPlannedDuration--}
```
public final Duration getPlannedDuration()
```


Hämtar den ursprungliga eller planerade varaktigheten – den totala arbetstiden från uppgiftens planerade startdatum till det planerade slutdatumet.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the original or planned duration -- the total working time from the task planned start date to the planned finish date.
### getPrimaryConstraintDate() {#getPrimaryConstraintDate--}
```
public final Date getPrimaryConstraintDate()
```


Hämtar datumet för primär begränsning.

**Returns:**
java.util.Date - datumet för primär begränsning.
### getPrimaryConstraintType() {#getPrimaryConstraintType--}
```
public final int getPrimaryConstraintType()
```


Hämtar en typ av primär begränsning.

**Returns:**
int - en typ av primär begränsning.
### getRawActivityType() {#getRawActivityType--}
```
public final String getRawActivityType()
```


Hämtar råtextrepresentation (som i källfilen) av fältet 'Activity Type' för aktiviteten.

--------------------

Gäller endast för aktiviteter (icke‑sammanfattande uppgifter).

**Returns:**
java.lang.String - rå textrepresentation (som i källfilen) av fältet 'Activity Type' för aktiviteten.
### getRawCompletePercentType() {#getRawCompletePercentType--}
```
public final String getRawCompletePercentType()
```


Hämtar råtextrepresentation (som i källfilen) av fältet '% Complete Type' för aktiviteten.

--------------------

Gäller endast för aktiviteter (icke‑sammanfattande uppgifter).

**Returns:**
java.lang.String - rå textrepresentation (som i källfilen) av fältet '% Complete Type' för aktiviteten.
### getRawDurationType() {#getRawDurationType--}
```
public final String getRawDurationType()
```


Hämtar råtextrepresentation (som i källfilen) av fältet 'Duration Type' för aktiviteten.

--------------------

Gäller endast för aktiviteter (icke‑sammanfattande uppgifter).

**Returns:**
java.lang.String - rå textrepresentation (som i källfilen) av fältet 'Duration Type' för aktiviteten.
### getRawStatus() {#getRawStatus--}
```
public final String getRawStatus()
```


Hämtar råtextrepresentation (som i källfilen) av fältet 'Status' för aktiviteten.

--------------------

Gäller endast för aktiviteter (icke‑sammanfattande uppgifter).

**Returns:**
java.lang.String - rå textrepresentation (som i källfilen) av fältet 'Status' för aktiviteten.
### getRemainingEarlyFinish() {#getRemainingEarlyFinish--}
```
public final Date getRemainingEarlyFinish()
```


Hämtar återstående tidigt avslutsdatum - datumet då det återstående arbetet för aktiviteten är planerat att avslutas.

**Returns:**
java.util.Date - återstående tidiga slutdatum - datumet då återstående arbete för aktiviteten är planerat att slutföras.
### getRemainingEarlyStart() {#getRemainingEarlyStart--}
```
public final Date getRemainingEarlyStart()
```


Hämtar återstående tidigt startdatum - datumet då det återstående arbetet för aktiviteten är planerat att påbörjas.

**Returns:**
java.util.Date - återstående tidiga startdatum - datumet då återstående arbete för aktiviteten är planerat att påbörjas.
### getRemainingExpenseCost() {#getRemainingExpenseCost--}
```
public final BigDecimal getRemainingExpenseCost()
```


Hämtar värdet av återstående utgiftkostnad.

**Returns:**
java.math.BigDecimal - värdet av återstående utgift.
### getRemainingLaborUnits() {#getRemainingLaborUnits--}
```
public final double getRemainingLaborUnits()
```


Hämtar värdet av återstående arbetsenheter.

**Returns:**
double - värdet av återstående arbetsenheter.
### getRemainingLateFinish() {#getRemainingLateFinish--}
```
public final Date getRemainingLateFinish()
```


Hämtar återstående sent avslutsdatum.

**Returns:**
java.util.Date - återstående sena slutdatum.
### getRemainingLateStart() {#getRemainingLateStart--}
```
public final Date getRemainingLateStart()
```


Hämtar återstående sent startdatum.

**Returns:**
java.util.Date - återstående sena startdatum.
### getRemainingNonLaborUnits() {#getRemainingNonLaborUnits--}
```
public final double getRemainingNonLaborUnits()
```


Hämtar värdet av återstående icke‑arbetsenheter.

**Returns:**
double - värdet av återstående icke-arbetsenheter.
### getSecondaryConstraintDate() {#getSecondaryConstraintDate--}
```
public final Date getSecondaryConstraintDate()
```


Hämtar datumet för sekundär begränsning.

**Returns:**
java.util.Date - datumet för sekundär begränsning.
### getSecondaryConstraintType() {#getSecondaryConstraintType--}
```
public final int getSecondaryConstraintType()
```


Hämtar en typ av sekundär begränsning.

**Returns:**
int - en typ av sekundär begränsning.
### getSequenceNumber() {#getSequenceNumber--}
```
public final int getSequenceNumber()
```


Hämtar sekvensnumret för WBS‑objektet (sammanfattande uppgifter). Det används för att sortera sammanfattande uppgifter i Primavera.

--------------------

Gäller för WBS‑objekt (sammanfattande uppgifter).

**Returns:**
int – sekvensnumret för WBS‑objektet (sammanfattande uppgifter).
### getUnitsPercentComplete() {#getUnitsPercentComplete--}
```
public final double getUnitsPercentComplete()
```


Hämtar värdet av enheternas procentuella slutförande.

**Returns:**
double – värdet för enheternas procentuella slutförande.
