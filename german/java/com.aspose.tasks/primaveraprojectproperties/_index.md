---
title: "PrimaveraProjectProperties"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt Primavera-spezifische Eigenschaften für ein Projekt dar, das aus Primavera-Dateien XER oder P6XML gelesen wurde."
type: docs
weight: 205
url: /de/java/com.aspose.tasks/primaveraprojectproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectProperties
```

Stellt Primavera-spezifische Eigenschaften für ein Projekt dar, das aus Primavera-Dateien (XER oder P6XML) gelesen wurde.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getBaselineProjects()](#getBaselineProjects--) | Ruft das Array von Basislinienprojekten des aktuellen Projekts ab. |
| [getCriticalActivitiesDefiningMethod()](#getCriticalActivitiesDefiningMethod--) | Ruft die Methode zur Definition kritischer Aktivitäten ab: Längster Pfad oder Total Float-Ansatz. |
| [getCriticalTotalFloatLimit()](#getCriticalTotalFloatLimit--) | Ruft den Schwellenwert ab, der zur Definition kritischer Aktivitäten verwendet wird, wenn die TotalFloat-Methode eingesetzt wird. |
| [getCurrentBaselineProjectId()](#getCurrentBaselineProjectId--) | Ruft die ID des aktuellen Basislinienprojekts ab. |
| [getIgnoreOtherProjectRelationships()](#getIgnoreOtherProjectRelationships--) | Ruft ein Flag ab, das festlegt, ob Aktivitätsbeziehungen zwischen Projekten ignoriert werden sollen. |
| [getMakeOpenEndedActivitiesCritical()](#getMakeOpenEndedActivitiesCritical--) | Ruft ein Flag ab, das festlegt, ob Aktivitäten beim Planen des Projekts als kritisch markiert werden sollen. |
| [getRelationshipLagCalendar()](#getRelationshipLagCalendar--) | Ruft eine Option ab, die festlegt, welcher Kalender für die Terminierung von Beziehungsverzögerungen in Primavera-Projekten verwendet wird. |
| [getShortName()](#getShortName--) | Ruft den Kurznamen des Projekts (Projekt‑ID) ab. |
| [getUseExpectedFinishDates()](#getUseExpectedFinishDates--) | Ruft ein Flag ab, das festlegt, ob Aktivitätsenddaten als erwartete Enddaten geplant werden sollen. |
### getBaselineProjects() {#getBaselineProjects--}
```
public final Project[] getBaselineProjects()
```


Ruft das Array von Basislinienprojekten des aktuellen Projekts ab. Gilt für Projekte, die aus Primavera-XML-Dateien mit exportierten Basislinien gelesen wurden.

**Returns:**
com.aspose.tasks.Project[] - Array von Basislinienprojekten des aktuellen Projekts.
### getCriticalActivitiesDefiningMethod() {#getCriticalActivitiesDefiningMethod--}
```
public final int getCriticalActivitiesDefiningMethod()
```


Ruft die Methode zur Definition kritischer Aktivitäten ab: Längster Pfad oder Total Float-Ansatz.

**Returns:**
int - die Methode zur Definition kritischer Aktivitäten: Längster Pfad oder Total Float-Ansatz.
### getCriticalTotalFloatLimit() {#getCriticalTotalFloatLimit--}
```
public final Double getCriticalTotalFloatLimit()
```


Ruft den Schwellenwert ab, der zur Definition kritischer Aktivitäten verwendet wird, wenn die TotalFloat-Methode eingesetzt wird.

**Returns:**
java.lang.Double - der Schwellenwert, der zur Definition kritischer Aktivitäten verwendet wird, wenn die TotalFloat-Methode eingesetzt wird.
### getCurrentBaselineProjectId() {#getCurrentBaselineProjectId--}
```
public final int getCurrentBaselineProjectId()
```


Ruft die ID des aktuellen Basislinienprojekts ab. Gilt für Projekte, die aus Primavera-XML-Dateien mit exportierten Basislinien gelesen wurden.

**Returns:**
int - ID des aktuellen Basislinienprojekts.
### getIgnoreOtherProjectRelationships() {#getIgnoreOtherProjectRelationships--}
```
public final boolean getIgnoreOtherProjectRelationships()
```


Ruft ein Flag ab, das festlegt, ob Aktivitätsbeziehungen zwischen Projekten ignoriert werden sollen.

**Returns:**
boolean - ein Flag, das festlegt, ob Aktivitätsbeziehungen zwischen Projekten ignoriert werden sollen.
### getMakeOpenEndedActivitiesCritical() {#getMakeOpenEndedActivitiesCritical--}
```
public final boolean getMakeOpenEndedActivitiesCritical()
```


Ruft ein Flag ab, das festlegt, ob Aktivitäten beim Planen des Projekts als kritisch markiert werden sollen.

**Returns:**
boolean - ein Flag, das festlegt, ob Aktivitäten beim Planen des Projekts als kritisch markiert werden sollen.
### getRelationshipLagCalendar() {#getRelationshipLagCalendar--}
```
public final int getRelationshipLagCalendar()
```


Ruft eine Option ab, die festlegt, welcher Kalender für die Terminierung von Beziehungsverzögerungen in Primavera-Projekten verwendet wird.

**Returns:**
int - eine Option, die festlegt, welcher Kalender für die Terminierung von Beziehungsverzögerungen in Primavera-Projekten verwendet wird.
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Ruft den Kurznamen des Projekts (Projekt‑ID) ab.

**Returns:**
java.lang.String - Kurzname des Projekts (Projekt‑ID).
### getUseExpectedFinishDates() {#getUseExpectedFinishDates--}
```
public final boolean getUseExpectedFinishDates()
```


Ruft ein Flag ab, das festlegt, ob Aktivitätsenddaten als erwartete Enddaten geplant werden sollen.

**Returns:**
boolean - ein Flag, das festlegt, ob Aktivitätsenddaten als erwartete Enddaten geplant werden sollen.
