---
title: "PrimaveraTaskProperties"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Vertegenwoordigt Primavera-specifieke eigenschappen voor een taak die gelezen is uit Primavera-bestanden XER of P6XML."
type: docs
weight: 209
url: /nl/java/com.aspose.tasks/primaverataskproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraTaskProperties
```

Geeft Primavera-specifieke eigenschappen weer voor een taak gelezen uit Primavera-bestanden (XER of P6XML).
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getActivityId()](#getActivityId--) | Haalt een activiteit-id-veld op – de unieke identifier van een taak die door Primavera wordt gebruikt. |
| [getActivityType()](#getActivityType--) | Haalt de waarde van het veld 'Activity Type' op. |
| [getActualExpenseCost()](#getActualExpenseCost--) | Haalt de waarde van de werkelijke onkostenkosten op. |
| [getActualLaborCost()](#getActualLaborCost--) | Haalt de waarde van de werkelijke arbeidskosten op . |
| [getActualLaborUnits()](#getActualLaborUnits--) | Haalt de waarde van de werkelijke arbeidseenheden op. |
| [getActualMaterialCost()](#getActualMaterialCost--) | Haalt de waarde van de werkelijke materiaalkosten op. |
| [getActualNonLaborUnits()](#getActualNonLaborUnits--) | Haalt de waarde van de werkelijke niet-arbeidseenheden op. |
| [getActualNonlaborCost()](#getActualNonlaborCost--) | Haalt de waarde van de werkelijke niet-arbeidskosten op . |
| [getActualTotalCost()](#getActualTotalCost--) | Haalt de totale waarde van de werkelijke kosten op. |
| [getBudgetedExpenseCost()](#getBudgetedExpenseCost--) | Haalt de waarde van begrote (of geplande) uitgavenkosten op. |
| [getBudgetedLaborCost()](#getBudgetedLaborCost--) | Haalt de waarde van begrote (of geplande) arbeidskosten op . |
| [getBudgetedMaterialCost()](#getBudgetedMaterialCost--) | Haalt de waarde van van begrote (of geplande) materiaalkosten op. |
| [getBudgetedNonlaborCost()](#getBudgetedNonlaborCost--) | Haalt de waarde van begrote (of geplande) niet-arbeidskosten op . |
| [getBudgetedTotalCost()](#getBudgetedTotalCost--) | Haalt de totale waarde van begrote (of geplande) kosten op. |
| [getDurationPercentComplete()](#getDurationPercentComplete--) | Haalt de waarde van het voltooid percentage van de duur op. |
| [getDurationType()](#getDurationType--) | Haalt de waarde van het veld 'Duration Type' van de activiteit op. |
| [getPercentCompleteType()](#getPercentCompleteType--) | Haalt de waarde van het veld '% Complete Type' van de activiteit op. |
| [getPhysicalPercentComplete()](#getPhysicalPercentComplete--) | Haalt de waarde van Physical Percent Complete op. |
| [getPlannedDuration()](#getPlannedDuration--) | Haalt de oorspronkelijke of geplande duur op -- de totale werktijd van de geplande startdatum van de taak tot de geplande einddatum.. |
| [getPrimaryConstraintDate()](#getPrimaryConstraintDate--) | Haalt de datum van de primaire beperking op. |
| [getPrimaryConstraintType()](#getPrimaryConstraintType--) | Haalt een type van de primaire beperking op. |
| [getRawActivityType()](#getRawActivityType--) | Haalt de ruwe tekstrepresentatie (zoals in bronbestand) van het veld 'Activity Type' van de activiteit op. |
| [getRawCompletePercentType()](#getRawCompletePercentType--) | Haalt de ruwe tekstrepresentatie (zoals in bronbestand) van het veld '% Complete Type' van de activiteit op. |
| [getRawDurationType()](#getRawDurationType--) | Haalt de ruwe tekstrepresentatie (zoals in bronbestand) van het veld 'Duration Type' van de activiteit op. |
| [getRawStatus()](#getRawStatus--) | Haalt de ruwe tekstrepresentatie (zoals in bronbestand) van het veld 'Status' van de activiteit op. |
| [getRemainingEarlyFinish()](#getRemainingEarlyFinish--) | Haalt de resterende vroegste einddatum op - de datum waarop het resterende werk voor de activiteit gepland is om te worden voltooid. |
| [getRemainingEarlyStart()](#getRemainingEarlyStart--) | Haalt de resterende vroegste startdatum op - de datum waarop het resterende werk voor de activiteit gepland is om te beginnen. |
| [getRemainingExpenseCost()](#getRemainingExpenseCost--) | Haalt de waarde van de resterende uitgavenkosten op. |
| [getRemainingLaborUnits()](#getRemainingLaborUnits--) | Haalt de waarde van de resterende arbeidsunits op. |
| [getRemainingLateFinish()](#getRemainingLateFinish--) | Haalt de resterende laatste einddatum op. |
| [getRemainingLateStart()](#getRemainingLateStart--) | Haalt de resterende laatste startdatum op. |
| [getRemainingNonLaborUnits()](#getRemainingNonLaborUnits--) | Haalt de waarde van de resterende niet-arbeidsunits op. |
| [getSecondaryConstraintDate()](#getSecondaryConstraintDate--) | Haalt de datum van de secundaire beperking op. |
| [getSecondaryConstraintType()](#getSecondaryConstraintType--) | Haalt een type van de secundaire beperking op. |
| [getSequenceNumber()](#getSequenceNumber--) | Haalt het volgnummer van het WBS-item (samenvattende taken) op. |
| [getUnitsPercentComplete()](#getUnitsPercentComplete--) | Haalt de waarde van het percentage voltooid van eenheden op. |
### getActivityId() {#getActivityId--}
```
public final String getActivityId()
```


Haalt een activiteit-id-veld op – de unieke identifier van een taak die door Primavera wordt gebruikt.

--------------------

Alleen van toepassing op activiteiten (niet-samenvattende taken).

**Returns:**
java.lang.String - een activiteit-id-veld - de unieke identifier van een taak die door Primavera wordt gebruikt.
### getActivityType() {#getActivityType--}
```
public final int getActivityType()
```


Haalt de waarde van het veld 'Activity Type' op.

--------------------

Alleen van toepassing op activiteiten (niet-samenvattende taken).

**Returns:**
int - de waarde van het veld 'Activity Type'.
### getActualExpenseCost() {#getActualExpenseCost--}
```
public final BigDecimal getActualExpenseCost()
```


Haalt de waarde van de werkelijke onkostenkosten op.

**Returns:**
java.math.BigDecimal - de waarde van de werkelijke uitgavenkosten.
### getActualLaborCost() {#getActualLaborCost--}
```
public final BigDecimal getActualLaborCost()
```


Haalt de waarde van de werkelijke arbeidskosten op .

**Returns:**
java.math.BigDecimal - de waarde van de werkelijke arbeidskosten.
### getActualLaborUnits() {#getActualLaborUnits--}
```
public final double getActualLaborUnits()
```


Haalt de waarde van de werkelijke arbeidseenheden op.

**Returns:**
double - de waarde van de werkelijke arbeidsunits.
### getActualMaterialCost() {#getActualMaterialCost--}
```
public final BigDecimal getActualMaterialCost()
```


Haalt de waarde van de werkelijke materiaalkosten op.

**Returns:**
java.math.BigDecimal - de waarde van de werkelijke materiaalkosten.
### getActualNonLaborUnits() {#getActualNonLaborUnits--}
```
public final double getActualNonLaborUnits()
```


Haalt de waarde van de werkelijke niet-arbeidseenheden op.

**Returns:**
double - de waarde van de werkelijke niet-arbeidsunits.
### getActualNonlaborCost() {#getActualNonlaborCost--}
```
public final BigDecimal getActualNonlaborCost()
```


Haalt de waarde van de werkelijke niet-arbeidskosten op .

**Returns:**
java.math.BigDecimal - de waarde van de werkelijke niet-arbeidskosten.
### getActualTotalCost() {#getActualTotalCost--}
```
public final BigDecimal getActualTotalCost()
```


Haalt de totale waarde van de werkelijke kosten op.

**Returns:**
java.math.BigDecimal - de totale waarde van de werkelijke kosten.
### getBudgetedExpenseCost() {#getBudgetedExpenseCost--}
```
public final BigDecimal getBudgetedExpenseCost()
```


Haalt de waarde van begrote (of geplande) uitgavenkosten op.

**Returns:**
java.math.BigDecimal - de waarde van begrote (of geplande) uitgavenkosten.
### getBudgetedLaborCost() {#getBudgetedLaborCost--}
```
public final BigDecimal getBudgetedLaborCost()
```


Haalt de waarde van begrote (of geplande) arbeidskosten op .

**Returns:**
java.math.BigDecimal - de waarde van begrote (of geplande) arbeidskosten.
### getBudgetedMaterialCost() {#getBudgetedMaterialCost--}
```
public final BigDecimal getBudgetedMaterialCost()
```


Haalt de waarde van van begrote (of geplande) materiaalkosten op.

**Returns:**
java.math.BigDecimal - de waarde van begrote (of geplande) materiaalkosten.
### getBudgetedNonlaborCost() {#getBudgetedNonlaborCost--}
```
public final BigDecimal getBudgetedNonlaborCost()
```


Haalt de waarde van begrote (of geplande) niet-arbeidskosten op .

**Returns:**
java.math.BigDecimal - de waarde van begrote (of geplande) niet-arbeidskosten.
### getBudgetedTotalCost() {#getBudgetedTotalCost--}
```
public final BigDecimal getBudgetedTotalCost()
```


Haalt de totale waarde van begrote (of geplande) kosten op.

**Returns:**
java.math.BigDecimal - de totale waarde van begrote (of geplande) kosten.
### getDurationPercentComplete() {#getDurationPercentComplete--}
```
public final double getDurationPercentComplete()
```


Haalt de waarde van het voltooid percentage van de duur op.

**Returns:**
double - de waarde van het percentage voltooid van de duur.
### getDurationType() {#getDurationType--}
```
public final int getDurationType()
```


Haalt de waarde van het veld 'Duration Type' van de activiteit op.

--------------------

Alleen van toepassing op activiteiten (niet-samenvattende taken).

**Returns:**
int - de waarde van het veld 'Duration Type' van de activiteit.
### getPercentCompleteType() {#getPercentCompleteType--}
```
public final int getPercentCompleteType()
```


Haalt de waarde van het veld '% Complete Type' van de activiteit op.

--------------------

Alleen van toepassing op activiteiten (niet-samenvattende taken).

**Returns:**
int - de waarde van het veld '% Complete Type' van de activiteit.
### getPhysicalPercentComplete() {#getPhysicalPercentComplete--}
```
public final double getPhysicalPercentComplete()
```


Haalt de waarde van Physical Percent Complete op.

--------------------

Alleen van toepassing op activiteiten (niet-samenvattende taken).

**Returns:**
double - de waarde van Physical Percent Complete.
### getPlannedDuration() {#getPlannedDuration--}
```
public final Duration getPlannedDuration()
```


Haalt de oorspronkelijke of geplande duur op -- de totale werktijd van de geplande startdatum van de taak tot de geplande einddatum..

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the original or planned duration -- the total working time from the task planned start date to the planned finish date.
### getPrimaryConstraintDate() {#getPrimaryConstraintDate--}
```
public final Date getPrimaryConstraintDate()
```


Haalt de datum van de primaire beperking op.

**Returns:**
java.util.Date - de datum van de primaire beperking.
### getPrimaryConstraintType() {#getPrimaryConstraintType--}
```
public final int getPrimaryConstraintType()
```


Haalt een type van de primaire beperking op.

**Returns:**
int - een type van de primaire beperking.
### getRawActivityType() {#getRawActivityType--}
```
public final String getRawActivityType()
```


Haalt de ruwe tekstrepresentatie (zoals in bronbestand) van het veld 'Activity Type' van de activiteit op.

--------------------

Alleen van toepassing op activiteiten (niet-samenvattende taken).

**Returns:**
java.lang.String - ruwe tekstrepresentatie (zoals in bronbestand) van het veld 'Activity Type' van de activiteit.
### getRawCompletePercentType() {#getRawCompletePercentType--}
```
public final String getRawCompletePercentType()
```


Haalt de ruwe tekstrepresentatie (zoals in bronbestand) van het veld '% Complete Type' van de activiteit op.

--------------------

Alleen van toepassing op activiteiten (niet-samenvattende taken).

**Returns:**
java.lang.String - ruwe tekstrepresentatie (zoals in bronbestand) van het veld '% Complete Type' van de activiteit.
### getRawDurationType() {#getRawDurationType--}
```
public final String getRawDurationType()
```


Haalt de ruwe tekstrepresentatie (zoals in bronbestand) van het veld 'Duration Type' van de activiteit op.

--------------------

Alleen van toepassing op activiteiten (niet-samenvattende taken).

**Returns:**
java.lang.String - ruwe tekstrepresentatie (zoals in bronbestand) van het veld 'Duration Type' van de activiteit.
### getRawStatus() {#getRawStatus--}
```
public final String getRawStatus()
```


Haalt de ruwe tekstrepresentatie (zoals in bronbestand) van het veld 'Status' van de activiteit op.

--------------------

Alleen van toepassing op activiteiten (niet-samenvattende taken).

**Returns:**
java.lang.String - ruwe tekstrepresentatie (zoals in bronbestand) van het veld 'Status' van de activiteit.
### getRemainingEarlyFinish() {#getRemainingEarlyFinish--}
```
public final Date getRemainingEarlyFinish()
```


Haalt de resterende vroegste einddatum op - de datum waarop het resterende werk voor de activiteit gepland is om te worden voltooid.

**Returns:**
java.util.Date - resterende vroegste einddatum - de datum waarop het resterende werk voor de activiteit gepland is om te worden afgerond.
### getRemainingEarlyStart() {#getRemainingEarlyStart--}
```
public final Date getRemainingEarlyStart()
```


Haalt de resterende vroegste startdatum op - de datum waarop het resterende werk voor de activiteit gepland is om te beginnen.

**Returns:**
java.util.Date - resterende vroegste startdatum - de datum waarop het resterende werk voor de activiteit gepland is om te beginnen.
### getRemainingExpenseCost() {#getRemainingExpenseCost--}
```
public final BigDecimal getRemainingExpenseCost()
```


Haalt de waarde van de resterende uitgavenkosten op.

**Returns:**
java.math.BigDecimal - de waarde van de resterende uitgavenkosten.
### getRemainingLaborUnits() {#getRemainingLaborUnits--}
```
public final double getRemainingLaborUnits()
```


Haalt de waarde van de resterende arbeidsunits op.

**Returns:**
double - de waarde van de resterende arbeidseenheden.
### getRemainingLateFinish() {#getRemainingLateFinish--}
```
public final Date getRemainingLateFinish()
```


Haalt de resterende laatste einddatum op.

**Returns:**
java.util.Date - resterende late einddatum.
### getRemainingLateStart() {#getRemainingLateStart--}
```
public final Date getRemainingLateStart()
```


Haalt de resterende laatste startdatum op.

**Returns:**
java.util.Date - resterende late startdatum.
### getRemainingNonLaborUnits() {#getRemainingNonLaborUnits--}
```
public final double getRemainingNonLaborUnits()
```


Haalt de waarde van de resterende niet-arbeidsunits op.

**Returns:**
double - de waarde van de resterende niet-arbeidseenheden.
### getSecondaryConstraintDate() {#getSecondaryConstraintDate--}
```
public final Date getSecondaryConstraintDate()
```


Haalt de datum van de secundaire beperking op.

**Returns:**
java.util.Date - de datum van de secundaire beperking.
### getSecondaryConstraintType() {#getSecondaryConstraintType--}
```
public final int getSecondaryConstraintType()
```


Haalt een type van de secundaire beperking op.

**Returns:**
int - een type van de secundaire beperking.
### getSequenceNumber() {#getSequenceNumber--}
```
public final int getSequenceNumber()
```


Haalt het volgnummer op van het WBS-item (samenvattende taken). Het wordt gebruikt om samenvattende taken in Primavera te sorteren.

--------------------

Van toepassing op WBS-items (samenvattende taken).

**Returns:**
int - het volgnummer van het WBS-item (samenvattende taken).
### getUnitsPercentComplete() {#getUnitsPercentComplete--}
```
public final double getUnitsPercentComplete()
```


Haalt de waarde van het percentage voltooid van eenheden op.

**Returns:**
double - de waarde van units percent complete.
