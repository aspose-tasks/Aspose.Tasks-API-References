---
title: "PrimaveraProjectProperties"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar Primavera‑specifika egenskaper för ett projekt läst från Primavera‑filer XER eller P6XML."
type: docs
weight: 205
url: /sv/java/com.aspose.tasks/primaveraprojectproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectProperties
```

Representerar Primavera-specifika egenskaper för ett projekt som lästs från Primavera-filer (XER eller P6XML).
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getBaselineProjects()](#getBaselineProjects--) | Hämtar array med baslinjeprojekt för det aktuella projektet. |
| [getCriticalActivitiesDefiningMethod()](#getCriticalActivitiesDefiningMethod--) | Hämtar metoden för att definiera kritiska aktiviteter: Längsta vägen eller Total Float‑metoden. |
| [getCriticalTotalFloatLimit()](#getCriticalTotalFloatLimit--) | Hämtar tröskelvärdet som används för att definiera kritiska aktiviteter om TotalFloat‑metoden används. |
| [getCurrentBaselineProjectId()](#getCurrentBaselineProjectId--) | Hämtar Id för det aktuella baslinjeprojektet. |
| [getIgnoreOtherProjectRelationships()](#getIgnoreOtherProjectRelationships--) | Hämtar en flagga som definierar om aktivitetsrelationer mellan projekt ska ignoreras. |
| [getMakeOpenEndedActivitiesCritical()](#getMakeOpenEndedActivitiesCritical--) | Hämtar en flagga som definierar om aktiviteter ska markeras som kritiska när projektet schemaläggs. |
| [getRelationshipLagCalendar()](#getRelationshipLagCalendar--) | Hämtar ett alternativ som definierar vilken kalender som ska användas för schemaläggning av relationsfördröjning i Primavera-projekt. |
| [getShortName()](#getShortName--) | Hämtar projektets korta namn (Projekt-ID). |
| [getUseExpectedFinishDates()](#getUseExpectedFinishDates--) | Hämtar en flagga som definierar om aktiviteters slutdatum ska schemaläggas som de förväntade slutdatumen. |
### getBaselineProjects() {#getBaselineProjects--}
```
public final Project[] getBaselineProjects()
```


Hämtar en array av baslinjeprojekt för det aktuella projektet. Gäller för projekt som läses från Primavera XML-filer som innehåller exporterade baslinjer.

**Returns:**
com.aspose.tasks.Project[] - array av baslinjeprojekt för det aktuella projektet.
### getCriticalActivitiesDefiningMethod() {#getCriticalActivitiesDefiningMethod--}
```
public final int getCriticalActivitiesDefiningMethod()
```


Hämtar metoden för att definiera kritiska aktiviteter: Längsta vägen eller Total Float‑metoden.

**Returns:**
int - metoden för att definiera kritiska aktiviteter: Längsta vägen eller Total Float‑metoden.
### getCriticalTotalFloatLimit() {#getCriticalTotalFloatLimit--}
```
public final Double getCriticalTotalFloatLimit()
```


Hämtar tröskelvärdet som används för att definiera kritiska aktiviteter om TotalFloat‑metoden används.

**Returns:**
java.lang.Double - tröskelvärdet som används för att definiera kritiska aktiviteter om TotalFloat‑metoden används.
### getCurrentBaselineProjectId() {#getCurrentBaselineProjectId--}
```
public final int getCurrentBaselineProjectId()
```


Hämtar ID för det aktuella baslinjeprojektet. Gäller för projekt som läses från Primavera XML-filer som innehåller exporterade baslinjer.

**Returns:**
int - ID för det aktuella baslinjeprojektet.
### getIgnoreOtherProjectRelationships() {#getIgnoreOtherProjectRelationships--}
```
public final boolean getIgnoreOtherProjectRelationships()
```


Hämtar en flagga som definierar om aktivitetsrelationer mellan projekt ska ignoreras.

**Returns:**
boolean - en flagga som definierar om aktivitetsrelationer mellan projekt ska ignoreras.
### getMakeOpenEndedActivitiesCritical() {#getMakeOpenEndedActivitiesCritical--}
```
public final boolean getMakeOpenEndedActivitiesCritical()
```


Hämtar en flagga som definierar om aktiviteter ska markeras som kritiska när projektet schemaläggs.

**Returns:**
boolean - en flagga som definierar om aktiviteter ska markeras som kritiska när projektet schemaläggs.
### getRelationshipLagCalendar() {#getRelationshipLagCalendar--}
```
public final int getRelationshipLagCalendar()
```


Hämtar ett alternativ som definierar vilken kalender som ska användas för schemaläggning av relationsfördröjning i Primavera-projekt.

**Returns:**
int - ett alternativ som definierar vilken kalender som ska användas för schemaläggning av relationsfördröjning i Primavera-projekt
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Hämtar projektets korta namn (Projekt-ID).

**Returns:**
java.lang.String - projektets korta namn (Projekt-ID).
### getUseExpectedFinishDates() {#getUseExpectedFinishDates--}
```
public final boolean getUseExpectedFinishDates()
```


Hämtar en flagga som definierar om aktiviteters slutdatum ska schemaläggas som de förväntade slutdatumen.

**Returns:**
boolean - en flagga som definierar om aktiviteters slutdatum ska schemaläggas som de förväntade slutdatumen.
