---
title: "PrimaveraProjectProperties"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta le proprietà specifiche di Primavera per un progetto letto dai file Primavera XER o P6XML."
type: docs
weight: 205
url: /it/java/com.aspose.tasks/primaveraprojectproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectProperties
```

Rappresenta le proprietà specifiche di Primavera per un progetto letto dai file Primavera (XER o P6XML).
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getBaselineProjects()](#getBaselineProjects--) | Restituisce l'array di progetti di baseline del progetto corrente. |
| [getCriticalActivitiesDefiningMethod()](#getCriticalActivitiesDefiningMethod--) | Restituisce il metodo per definire le attività critiche: approccio Longest Path o Total Float. |
| [getCriticalTotalFloatLimit()](#getCriticalTotalFloatLimit--) | Restituisce il valore soglia utilizzato per definire le attività critiche se viene usato il metodo TotalFloat. |
| [getCurrentBaselineProjectId()](#getCurrentBaselineProjectId--) | Restituisce l'Id del progetto di baseline corrente. |
| [getIgnoreOtherProjectRelationships()](#getIgnoreOtherProjectRelationships--) | Restituisce un flag che definisce se ignorare le relazioni di attività tra i progetti. |
| [getMakeOpenEndedActivitiesCritical()](#getMakeOpenEndedActivitiesCritical--) | Restituisce un flag che definisce se le attività devono essere contrassegnate come critiche durante la pianificazione del progetto. |
| [getRelationshipLagCalendar()](#getRelationshipLagCalendar--) | Restituisce un'opzione che definisce quale calendario utilizzare per la pianificazione del ritardo di relazione (Relationship Lag) nei progetti Primavera. |
| [getShortName()](#getShortName--) | Ottiene il nome breve del progetto (ID progetto). |
| [getUseExpectedFinishDates()](#getUseExpectedFinishDates--) | Restituisce un flag che definisce se le date di fine attività devono essere programmate come le date di fine previste. |
### getBaselineProjects() {#getBaselineProjects--}
```
public final Project[] getBaselineProjects()
```


Restituisce l'array di progetti di baseline del progetto corrente. È applicabile ai progetti letti da file XML di Primavera contenenti baseline esportate.

**Returns:**
com.aspose.tasks.Project[] - array di progetti di baseline del progetto corrente.
### getCriticalActivitiesDefiningMethod() {#getCriticalActivitiesDefiningMethod--}
```
public final int getCriticalActivitiesDefiningMethod()
```


Restituisce il metodo per definire le attività critiche: approccio Longest Path o Total Float.

**Returns:**
int - il metodo per definire le attività critiche: approccio Longest Path o Total Float.
### getCriticalTotalFloatLimit() {#getCriticalTotalFloatLimit--}
```
public final Double getCriticalTotalFloatLimit()
```


Restituisce il valore soglia utilizzato per definire le attività critiche se viene usato il metodo TotalFloat.

**Returns:**
java.lang.Double - il valore soglia utilizzato per definire le attività critiche se viene usato il metodo TotalFloat.
### getCurrentBaselineProjectId() {#getCurrentBaselineProjectId--}
```
public final int getCurrentBaselineProjectId()
```


Restituisce l'Id del progetto di baseline corrente. È applicabile ai progetti letti da file XML di Primavera contenenti baseline esportate.

**Returns:**
int - Id del progetto di baseline corrente.
### getIgnoreOtherProjectRelationships() {#getIgnoreOtherProjectRelationships--}
```
public final boolean getIgnoreOtherProjectRelationships()
```


Restituisce un flag che definisce se ignorare le relazioni di attività tra i progetti.

**Returns:**
boolean - un flag che definisce se ignorare le relazioni di attività tra i progetti.
### getMakeOpenEndedActivitiesCritical() {#getMakeOpenEndedActivitiesCritical--}
```
public final boolean getMakeOpenEndedActivitiesCritical()
```


Restituisce un flag che definisce se le attività devono essere contrassegnate come critiche durante la pianificazione del progetto.

**Returns:**
boolean - un flag che definisce se le attività devono essere contrassegnate come critiche durante la pianificazione del progetto.
### getRelationshipLagCalendar() {#getRelationshipLagCalendar--}
```
public final int getRelationshipLagCalendar()
```


Restituisce un'opzione che definisce quale calendario utilizzare per la pianificazione del ritardo di relazione (Relationship Lag) nei progetti Primavera.

**Returns:**
int - un'opzione che definisce quale calendario utilizzare per la pianificazione del ritardo di relazione nei progetti Primavera.
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Ottiene il nome breve del progetto (ID progetto).

**Returns:**
java.lang.String - nome breve del progetto (ID progetto).
### getUseExpectedFinishDates() {#getUseExpectedFinishDates--}
```
public final boolean getUseExpectedFinishDates()
```


Restituisce un flag che definisce se le date di fine attività devono essere programmate come le date di fine previste.

**Returns:**
boolean - un flag che definisce se le date di fine attività devono essere programmate come le date di fine previste.
