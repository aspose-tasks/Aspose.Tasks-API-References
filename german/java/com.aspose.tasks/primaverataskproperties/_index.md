---
title: "PrimaveraTaskProperties"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt Primavera-spezifische Eigenschaften für eine Aufgabe dar, die aus Primavera-Dateien XER oder P6XML gelesen werden."
type: docs
weight: 209
url: /de/java/com.aspose.tasks/primaverataskproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraTaskProperties
```

Stellt Primavera-spezifische Eigenschaften für eine Aufgabe dar, die aus Primavera-Dateien (XER oder P6XML) gelesen wurde.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getActivityId()](#getActivityId--) | Liefert ein Aktivitäts-ID-Feld - die eindeutige Kennung einer Aufgabe, die von Primavera verwendet wird. |
| [getActivityType()](#getActivityType--) | Liefert den Wert des Feldes 'Activity Type'. |
| [getActualExpenseCost()](#getActualExpenseCost--) | Liefert den Wert der tatsächlichen Ausgabenkosten. |
| [getActualLaborCost()](#getActualLaborCost--) | Liefert den Wert der tatsächlichen Arbeitskosten . |
| [getActualLaborUnits()](#getActualLaborUnits--) | Liefert den Wert der tatsächlichen Arbeitseinheiten. |
| [getActualMaterialCost()](#getActualMaterialCost--) | Liefert den Wert der tatsächlichen Materialkosten. |
| [getActualNonLaborUnits()](#getActualNonLaborUnits--) | Liefert den Wert der tatsächlichen Nicht-Arbeitseinheiten. |
| [getActualNonlaborCost()](#getActualNonlaborCost--) | Liefert den Wert der tatsächlichen Nicht-Arbeitskosten . |
| [getActualTotalCost()](#getActualTotalCost--) | Liefert den Gesamtwert der tatsächlichen Kosten. |
| [getBudgetedExpenseCost()](#getBudgetedExpenseCost--) | Liefert den Wert der budgetierten (oder geplanten) Ausgabenkosten. |
| [getBudgetedLaborCost()](#getBudgetedLaborCost--) | Liefert den Wert der budgetierten (oder geplanten) Arbeitskosten . |
| [getBudgetedMaterialCost()](#getBudgetedMaterialCost--) | Liefert den Wert der budgetierten (oder geplanten) Materialkosten. |
| [getBudgetedNonlaborCost()](#getBudgetedNonlaborCost--) | Liefert den Wert der budgetierten (oder geplanten) Nicht-Arbeitskosten . |
| [getBudgetedTotalCost()](#getBudgetedTotalCost--) | Liefert den Gesamtwert der budgetierten (oder geplanten) Kosten. |
| [getDurationPercentComplete()](#getDurationPercentComplete--) | Ermittelt den Wert des prozentualen Fortschritts der Dauer. |
| [getDurationType()](#getDurationType--) | Ermittelt den Wert des Feldes 'Duration Type' der Aktivität. |
| [getPercentCompleteType()](#getPercentCompleteType--) | Ermittelt den Wert des Feldes '% Complete Type' der Aktivität. |
| [getPhysicalPercentComplete()](#getPhysicalPercentComplete--) | Ermittelt den Wert von Physical Percent Complete. |
| [getPlannedDuration()](#getPlannedDuration--) | Ermittelt die ursprüngliche oder geplante Dauer – die gesamte Arbeitszeit vom geplanten Startdatum der Aufgabe bis zum geplanten Enddatum. |
| [getPrimaryConstraintDate()](#getPrimaryConstraintDate--) | Ermittelt das Datum der primären Einschränkung. |
| [getPrimaryConstraintType()](#getPrimaryConstraintType--) | Ermittelt einen Typ der primären Einschränkung. |
| [getRawActivityType()](#getRawActivityType--) | Ermittelt die Rohtextdarstellung (wie in der Quelldatei) des Feldes 'Activity Type' der Aktivität. |
| [getRawCompletePercentType()](#getRawCompletePercentType--) | Ermittelt die Rohtextdarstellung (wie in der Quelldatei) des Feldes '% Complete Type' der Aktivität. |
| [getRawDurationType()](#getRawDurationType--) | Ermittelt die Rohtextdarstellung (wie in der Quelldatei) des Feldes 'Duration Type' der Aktivität. |
| [getRawStatus()](#getRawStatus--) | Ermittelt die Rohtextdarstellung (wie in der Quelldatei) des Feldes 'Status' der Aktivität. |
| [getRemainingEarlyFinish()](#getRemainingEarlyFinish--) | Ermittelt das verbleibende frühe Enddatum – das Datum, an dem die verbleibende Arbeit für die Aktivität voraussichtlich abgeschlossen wird. |
| [getRemainingEarlyStart()](#getRemainingEarlyStart--) | Ermittelt das verbleibende frühe Startdatum – das Datum, an dem die verbleibende Arbeit für die Aktivität voraussichtlich beginnt. |
| [getRemainingExpenseCost()](#getRemainingExpenseCost--) | Ermittelt den Wert der verbleibenden Aufwandskosten. |
| [getRemainingLaborUnits()](#getRemainingLaborUnits--) | Ermittelt den Wert der verbleibenden Arbeitseinheiten. |
| [getRemainingLateFinish()](#getRemainingLateFinish--) | Ermittelt das verbleibende späte Enddatum. |
| [getRemainingLateStart()](#getRemainingLateStart--) | Ermittelt das verbleibende späte Startdatum. |
| [getRemainingNonLaborUnits()](#getRemainingNonLaborUnits--) | Ermittelt den Wert der verbleibenden nicht-arbeitsbezogenen Einheiten. |
| [getSecondaryConstraintDate()](#getSecondaryConstraintDate--) | Ermittelt das Datum der sekundären Einschränkung. |
| [getSecondaryConstraintType()](#getSecondaryConstraintType--) | Ermittelt einen Typ der sekundären Einschränkung. |
| [getSequenceNumber()](#getSequenceNumber--) | Ermittelt die Sequenznummer des WBS-Elements (Zusammenfassungsaufgaben). |
| [getUnitsPercentComplete()](#getUnitsPercentComplete--) | Ermittelt den Wert des prozentualen Fortschritts der Einheiten. |
### getActivityId() {#getActivityId--}
```
public final String getActivityId()
```


Liefert ein Aktivitäts-ID-Feld - die eindeutige Kennung einer Aufgabe, die von Primavera verwendet wird.

--------------------

Nur für Aktivitäten (nicht zusammenfassende Aufgaben) anwendbar.

**Returns:**
java.lang.String – ein Aktivitäts-ID-Feld – die eindeutige Kennung einer Aufgabe, die von Primavera verwendet wird.
### getActivityType() {#getActivityType--}
```
public final int getActivityType()
```


Liefert den Wert des Feldes 'Activity Type'.

--------------------

Nur für Aktivitäten (nicht zusammenfassende Aufgaben) anwendbar.

**Returns:**
int – der Wert des Feldes 'Activity Type'.
### getActualExpenseCost() {#getActualExpenseCost--}
```
public final BigDecimal getActualExpenseCost()
```


Liefert den Wert der tatsächlichen Ausgabenkosten.

**Returns:**
java.math.BigDecimal - der Wert der tatsächlichen Ausgabenkosten.
### getActualLaborCost() {#getActualLaborCost--}
```
public final BigDecimal getActualLaborCost()
```


Liefert den Wert der tatsächlichen Arbeitskosten .

**Returns:**
java.math.BigDecimal - der Wert der tatsächlichen Arbeitskosten.
### getActualLaborUnits() {#getActualLaborUnits--}
```
public final double getActualLaborUnits()
```


Liefert den Wert der tatsächlichen Arbeitseinheiten.

**Returns:**
double - der Wert der tatsächlichen Arbeitseinheiten.
### getActualMaterialCost() {#getActualMaterialCost--}
```
public final BigDecimal getActualMaterialCost()
```


Liefert den Wert der tatsächlichen Materialkosten.

**Returns:**
java.math.BigDecimal - der Wert der tatsächlichen Materialkosten.
### getActualNonLaborUnits() {#getActualNonLaborUnits--}
```
public final double getActualNonLaborUnits()
```


Liefert den Wert der tatsächlichen Nicht-Arbeitseinheiten.

**Returns:**
double - der Wert der tatsächlichen Nichtarbeits-Einheiten.
### getActualNonlaborCost() {#getActualNonlaborCost--}
```
public final BigDecimal getActualNonlaborCost()
```


Liefert den Wert der tatsächlichen Nicht-Arbeitskosten .

**Returns:**
java.math.BigDecimal - der Wert der tatsächlichen Nichtarbeitskosten.
### getActualTotalCost() {#getActualTotalCost--}
```
public final BigDecimal getActualTotalCost()
```


Liefert den Gesamtwert der tatsächlichen Kosten.

**Returns:**
java.math.BigDecimal - der Gesamtwert der tatsächlichen Kosten.
### getBudgetedExpenseCost() {#getBudgetedExpenseCost--}
```
public final BigDecimal getBudgetedExpenseCost()
```


Liefert den Wert der budgetierten (oder geplanten) Ausgabenkosten.

**Returns:**
java.math.BigDecimal - der Wert der budgetierten (oder geplanten) Ausgabenkosten.
### getBudgetedLaborCost() {#getBudgetedLaborCost--}
```
public final BigDecimal getBudgetedLaborCost()
```


Liefert den Wert der budgetierten (oder geplanten) Arbeitskosten .

**Returns:**
java.math.BigDecimal - der Wert der budgetierten (oder geplanten) Arbeitskosten.
### getBudgetedMaterialCost() {#getBudgetedMaterialCost--}
```
public final BigDecimal getBudgetedMaterialCost()
```


Liefert den Wert der budgetierten (oder geplanten) Materialkosten.

**Returns:**
java.math.BigDecimal - der Wert der budgetierten (oder geplanten) Materialkosten.
### getBudgetedNonlaborCost() {#getBudgetedNonlaborCost--}
```
public final BigDecimal getBudgetedNonlaborCost()
```


Liefert den Wert der budgetierten (oder geplanten) Nicht-Arbeitskosten .

**Returns:**
java.math.BigDecimal - der Wert der budgetierten (oder geplanten) Nichtarbeitskosten.
### getBudgetedTotalCost() {#getBudgetedTotalCost--}
```
public final BigDecimal getBudgetedTotalCost()
```


Liefert den Gesamtwert der budgetierten (oder geplanten) Kosten.

**Returns:**
java.math.BigDecimal - der Gesamtwert der budgetierten (oder geplanten) Kosten.
### getDurationPercentComplete() {#getDurationPercentComplete--}
```
public final double getDurationPercentComplete()
```


Ermittelt den Wert des prozentualen Fortschritts der Dauer.

**Returns:**
double - der Wert des prozentualen Abschlusses der Dauer.
### getDurationType() {#getDurationType--}
```
public final int getDurationType()
```


Ermittelt den Wert des Feldes 'Duration Type' der Aktivität.

--------------------

Nur für Aktivitäten (nicht zusammenfassende Aufgaben) anwendbar.

**Returns:**
int - der Wert des Feldes 'Duration Type' der Aktivität.
### getPercentCompleteType() {#getPercentCompleteType--}
```
public final int getPercentCompleteType()
```


Ermittelt den Wert des Feldes '% Complete Type' der Aktivität.

--------------------

Nur für Aktivitäten (nicht zusammenfassende Aufgaben) anwendbar.

**Returns:**
int - der Wert des Feldes '% Complete Type' der Aktivität.
### getPhysicalPercentComplete() {#getPhysicalPercentComplete--}
```
public final double getPhysicalPercentComplete()
```


Ermittelt den Wert von Physical Percent Complete.

--------------------

Nur für Aktivitäten (nicht zusammenfassende Aufgaben) anwendbar.

**Returns:**
double - der Wert des physischen Prozentsatzes des Abschlusses.
### getPlannedDuration() {#getPlannedDuration--}
```
public final Duration getPlannedDuration()
```


Ermittelt die ursprüngliche oder geplante Dauer – die gesamte Arbeitszeit vom geplanten Startdatum der Aufgabe bis zum geplanten Enddatum.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the original or planned duration -- the total working time from the task planned start date to the planned finish date.
### getPrimaryConstraintDate() {#getPrimaryConstraintDate--}
```
public final Date getPrimaryConstraintDate()
```


Ermittelt das Datum der primären Einschränkung.

**Returns:**
java.util.Date - das Datum der primären Einschränkung.
### getPrimaryConstraintType() {#getPrimaryConstraintType--}
```
public final int getPrimaryConstraintType()
```


Ermittelt einen Typ der primären Einschränkung.

**Returns:**
int - ein Typ der primären Einschränkung.
### getRawActivityType() {#getRawActivityType--}
```
public final String getRawActivityType()
```


Ermittelt die Rohtextdarstellung (wie in der Quelldatei) des Feldes 'Activity Type' der Aktivität.

--------------------

Nur für Aktivitäten (nicht zusammenfassende Aufgaben) anwendbar.

**Returns:**
java.lang.String - Rohtextdarstellung (wie in der Quelldatei) des Feldes 'Activity Type' der Aktivität.
### getRawCompletePercentType() {#getRawCompletePercentType--}
```
public final String getRawCompletePercentType()
```


Ermittelt die Rohtextdarstellung (wie in der Quelldatei) des Feldes '% Complete Type' der Aktivität.

--------------------

Nur für Aktivitäten (nicht zusammenfassende Aufgaben) anwendbar.

**Returns:**
java.lang.String - Rohtextdarstellung (wie in der Quelldatei) des Feldes '% Complete Type' der Aktivität.
### getRawDurationType() {#getRawDurationType--}
```
public final String getRawDurationType()
```


Ermittelt die Rohtextdarstellung (wie in der Quelldatei) des Feldes 'Duration Type' der Aktivität.

--------------------

Nur für Aktivitäten (nicht zusammenfassende Aufgaben) anwendbar.

**Returns:**
java.lang.String - Rohtextdarstellung (wie in der Quelldatei) des Feldes 'Duration Type' der Aktivität.
### getRawStatus() {#getRawStatus--}
```
public final String getRawStatus()
```


Ermittelt die Rohtextdarstellung (wie in der Quelldatei) des Feldes 'Status' der Aktivität.

--------------------

Nur für Aktivitäten (nicht zusammenfassende Aufgaben) anwendbar.

**Returns:**
java.lang.String - Rohtextdarstellung (wie in der Quelldatei) des Feldes 'Status' der Aktivität.
### getRemainingEarlyFinish() {#getRemainingEarlyFinish--}
```
public final Date getRemainingEarlyFinish()
```


Ermittelt das verbleibende frühe Enddatum – das Datum, an dem die verbleibende Arbeit für die Aktivität voraussichtlich abgeschlossen wird.

**Returns:**
java.util.Date - verbleibendes frühestes Enddatum - das Datum, an dem die verbleibende Arbeit für die Aktivität voraussichtlich abgeschlossen wird.
### getRemainingEarlyStart() {#getRemainingEarlyStart--}
```
public final Date getRemainingEarlyStart()
```


Ermittelt das verbleibende frühe Startdatum – das Datum, an dem die verbleibende Arbeit für die Aktivität voraussichtlich beginnt.

**Returns:**
java.util.Date - verbleibendes frühestes Startdatum - das Datum, an dem die verbleibende Arbeit für die Aktivität voraussichtlich beginnt.
### getRemainingExpenseCost() {#getRemainingExpenseCost--}
```
public final BigDecimal getRemainingExpenseCost()
```


Ermittelt den Wert der verbleibenden Aufwandskosten.

**Returns:**
java.math.BigDecimal - der Wert der verbleibenden Ausgabenkosten.
### getRemainingLaborUnits() {#getRemainingLaborUnits--}
```
public final double getRemainingLaborUnits()
```


Ermittelt den Wert der verbleibenden Arbeitseinheiten.

**Returns:**
double - der Wert der verbleibenden Arbeitseinheiten.
### getRemainingLateFinish() {#getRemainingLateFinish--}
```
public final Date getRemainingLateFinish()
```


Ermittelt das verbleibende späte Enddatum.

**Returns:**
java.util.Date - verbleibendes spätes Enddatum.
### getRemainingLateStart() {#getRemainingLateStart--}
```
public final Date getRemainingLateStart()
```


Ermittelt das verbleibende späte Startdatum.

**Returns:**
java.util.Date - verbleibendes spätes Startdatum.
### getRemainingNonLaborUnits() {#getRemainingNonLaborUnits--}
```
public final double getRemainingNonLaborUnits()
```


Ermittelt den Wert der verbleibenden nicht-arbeitsbezogenen Einheiten.

**Returns:**
double - der Wert der verbleibenden Nicht-Arbeitseinheiten.
### getSecondaryConstraintDate() {#getSecondaryConstraintDate--}
```
public final Date getSecondaryConstraintDate()
```


Ermittelt das Datum der sekundären Einschränkung.

**Returns:**
java.util.Date - das Datum der sekundären Einschränkung.
### getSecondaryConstraintType() {#getSecondaryConstraintType--}
```
public final int getSecondaryConstraintType()
```


Ermittelt einen Typ der sekundären Einschränkung.

**Returns:**
int - ein Typ der sekundären Einschränkung.
### getSequenceNumber() {#getSequenceNumber--}
```
public final int getSequenceNumber()
```


Gibt die Sequenznummer des WBS-Elements (Zusammenfassungsaufgaben) zurück. Sie wird verwendet, um Zusammenfassungsaufgaben in Primavera zu sortieren.

--------------------

Anwendbar auf WBS-Elemente (Zusammenfassungsaufgaben).

**Returns:**
int - die Sequenznummer des WBS-Elements (Zusammenfassungsaufgaben).
### getUnitsPercentComplete() {#getUnitsPercentComplete--}
```
public final double getUnitsPercentComplete()
```


Ermittelt den Wert des prozentualen Fortschritts der Einheiten.

**Returns:**
double - der Wert des prozentualen Fertigstellungsgrades der Einheiten.
