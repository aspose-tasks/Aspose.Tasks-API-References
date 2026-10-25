---
title: "PrimaveraProjectProperties"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt Primavera‑specifieke eigenschappen voor een project voor die zijn gelezen uit Primavera‑bestanden XER of P6XML."
type: docs
weight: 205
url: /nl/java/com.aspose.tasks/primaveraprojectproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectProperties
```

Geeft Primavera-specifieke eigenschappen weer voor een project gelezen uit Primavera-bestanden (XER of P6XML).
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getBaselineProjects()](#getBaselineProjects--) | Haalt array op van baseline‑projecten van het huidige project. |
| [getCriticalActivitiesDefiningMethod()](#getCriticalActivitiesDefiningMethod--) | Haalt de methode op voor het definiëren van kritieke activiteiten: Langste pad of Total Float‑benadering. |
| [getCriticalTotalFloatLimit()](#getCriticalTotalFloatLimit--) | Haalt de drempelwaarde op die wordt gebruikt om kritieke activiteiten te definiëren als de TotalFloat‑methode wordt gebruikt. |
| [getCurrentBaselineProjectId()](#getCurrentBaselineProjectId--) | Haalt Id op van het huidige baseline‑project. |
| [getIgnoreOtherProjectRelationships()](#getIgnoreOtherProjectRelationships--) | Haalt een vlag op die bepaalt of activiteitsrelaties tussen projecten moeten worden genegeerd. |
| [getMakeOpenEndedActivitiesCritical()](#getMakeOpenEndedActivitiesCritical--) | Haalt een vlag op die bepaalt of activiteiten als kritisch gemarkeerd moeten worden bij het plannen van het project. |
| [getRelationshipLagCalendar()](#getRelationshipLagCalendar--) | Haalt een optie op die bepaalt welke kalender moet worden gebruikt voor het plannen van Relationship Lag in Primavera‑projecten. |
| [getShortName()](#getShortName--) | Haalt de korte naam van het project (Project-ID) op. |
| [getUseExpectedFinishDates()](#getUseExpectedFinishDates--) | Haalt een vlag op die bepaalt of einddatums van activiteiten moeten worden gepland als de verwachte einddatums. |
### getBaselineProjects() {#getBaselineProjects--}
```
public final Project[] getBaselineProjects()
```


Haalt array op van baseline‑projecten van het huidige project. Is van toepassing op projecten die zijn gelezen uit Primavera‑XML‑bestanden met geëxporteerde baselines.

**Returns:**
com.aspose.tasks.Project[] - array van baseline‑projecten van het huidige project.
### getCriticalActivitiesDefiningMethod() {#getCriticalActivitiesDefiningMethod--}
```
public final int getCriticalActivitiesDefiningMethod()
```


Haalt de methode op voor het definiëren van kritieke activiteiten: Langste pad of Total Float‑benadering.

**Returns:**
int - de methode voor het definiëren van kritieke activiteiten: Langste pad of Total Float‑benadering.
### getCriticalTotalFloatLimit() {#getCriticalTotalFloatLimit--}
```
public final Double getCriticalTotalFloatLimit()
```


Haalt de drempelwaarde op die wordt gebruikt om kritieke activiteiten te definiëren als de TotalFloat‑methode wordt gebruikt.

**Returns:**
java.lang.Double - de drempelwaarde die wordt gebruikt om kritieke activiteiten te definiëren als de TotalFloat‑methode wordt gebruikt.
### getCurrentBaselineProjectId() {#getCurrentBaselineProjectId--}
```
public final int getCurrentBaselineProjectId()
```


Haalt Id op van het huidige baseline‑project. Is van toepassing op projecten die zijn gelezen uit Primavera‑XML‑bestanden met geëxporteerde baselines.

**Returns:**
int - Id van het huidige baseline-project.
### getIgnoreOtherProjectRelationships() {#getIgnoreOtherProjectRelationships--}
```
public final boolean getIgnoreOtherProjectRelationships()
```


Haalt een vlag op die bepaalt of activiteitsrelaties tussen projecten moeten worden genegeerd.

**Returns:**
boolean - een vlag die bepaalt of activiteitrelaties tussen projecten genegeerd moeten worden.
### getMakeOpenEndedActivitiesCritical() {#getMakeOpenEndedActivitiesCritical--}
```
public final boolean getMakeOpenEndedActivitiesCritical()
```


Haalt een vlag op die bepaalt of activiteiten als kritisch gemarkeerd moeten worden bij het plannen van het project.

**Returns:**
boolean - een vlag die bepaalt of activiteiten gemarkeerd moeten worden als kritiek bij het plannen van het project.
### getRelationshipLagCalendar() {#getRelationshipLagCalendar--}
```
public final int getRelationshipLagCalendar()
```


Haalt een optie op die bepaalt welke kalender moet worden gebruikt voor het plannen van Relationship Lag in Primavera‑projecten.

**Returns:**
int - een optie die bepaalt welke agenda gebruikt moet worden voor het plannen van Relationship Lag in Primavera-projecten
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Haalt de korte naam van het project (Project-ID) op.

**Returns:**
java.lang.String - korte naam van het project (Project-ID).
### getUseExpectedFinishDates() {#getUseExpectedFinishDates--}
```
public final boolean getUseExpectedFinishDates()
```


Haalt een vlag op die bepaalt of einddatums van activiteiten moeten worden gepland als de verwachte einddatums.

**Returns:**
boolean - een vlag die bepaalt of einddatums van activiteiten gepland moeten worden als de verwachte einddatums.
