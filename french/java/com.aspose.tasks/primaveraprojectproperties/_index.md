---
title: "PrimaveraProjectProperties"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente les propriétés spécifiques à Primavera pour un projet lu à partir des fichiers Primavera XER ou P6XML."
type: docs
weight: 205
url: /fr/java/com.aspose.tasks/primaveraprojectproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectProperties
```

Représente les propriétés spécifiques à Primavera pour un projet lu à partir de fichiers Primavera (XER ou P6XML).
## Méthodes

| Méthode | Description |
| --- | --- |
| [getBaselineProjects()](#getBaselineProjects--) | Obtient le tableau des projets de référence du projet actuel. |
| [getCriticalActivitiesDefiningMethod()](#getCriticalActivitiesDefiningMethod--) | Obtient la méthode de définition des activités critiques : chemin le plus long ou approche du flottement total. |
| [getCriticalTotalFloatLimit()](#getCriticalTotalFloatLimit--) | Obtient la valeur seuil utilisée pour définir les activités critiques si la méthode TotalFloat est utilisée. |
| [getCurrentBaselineProjectId()](#getCurrentBaselineProjectId--) | Obtient l'ID du projet de référence actuel. |
| [getIgnoreOtherProjectRelationships()](#getIgnoreOtherProjectRelationships--) | Obtient un indicateur qui définit s'il faut ignorer les relations d'activité entre les projets. |
| [getMakeOpenEndedActivitiesCritical()](#getMakeOpenEndedActivitiesCritical--) | Obtient un indicateur qui définit si les activités doivent être marquées comme critiques lors de la planification du projet. |
| [getRelationshipLagCalendar()](#getRelationshipLagCalendar--) | Obtient une option qui définit quel calendrier utiliser pour planifier le retard de relation dans les projets Primavera. |
| [getShortName()](#getShortName--) | Obtient le nom court du projet (ID du projet). |
| [getUseExpectedFinishDates()](#getUseExpectedFinishDates--) | Obtient un indicateur qui définit si les dates de fin d'activité doivent être planifiées comme les dates de fin prévues. |
### getBaselineProjects() {#getBaselineProjects--}
```
public final Project[] getBaselineProjects()
```


Obtient le tableau des projets de référence du projet actuel. S'applique aux projets lus à partir de fichiers XML Primavera contenant des références exportées.

**Returns:**
com.aspose.tasks.Project[] - tableau des projets de référence du projet actuel.
### getCriticalActivitiesDefiningMethod() {#getCriticalActivitiesDefiningMethod--}
```
public final int getCriticalActivitiesDefiningMethod()
```


Obtient la méthode de définition des activités critiques : chemin le plus long ou approche du flottement total.

**Returns:**
int - la méthode de définition des activités critiques : chemin le plus long ou approche du flottement total.
### getCriticalTotalFloatLimit() {#getCriticalTotalFloatLimit--}
```
public final Double getCriticalTotalFloatLimit()
```


Obtient la valeur seuil utilisée pour définir les activités critiques si la méthode TotalFloat est utilisée.

**Returns:**
java.lang.Double - la valeur seuil utilisée pour définir les activités critiques si la méthode TotalFloat est utilisée.
### getCurrentBaselineProjectId() {#getCurrentBaselineProjectId--}
```
public final int getCurrentBaselineProjectId()
```


Obtient l'ID du projet de référence actuel. S'applique aux projets lus à partir de fichiers XML Primavera contenant des références exportées.

**Returns:**
int - Identifiant du projet de référence actuel.
### getIgnoreOtherProjectRelationships() {#getIgnoreOtherProjectRelationships--}
```
public final boolean getIgnoreOtherProjectRelationships()
```


Obtient un indicateur qui définit s'il faut ignorer les relations d'activité entre les projets.

**Returns:**
boolean - un indicateur qui définit s'il faut ignorer les relations d'activité entre les projets.
### getMakeOpenEndedActivitiesCritical() {#getMakeOpenEndedActivitiesCritical--}
```
public final boolean getMakeOpenEndedActivitiesCritical()
```


Obtient un indicateur qui définit si les activités doivent être marquées comme critiques lors de la planification du projet.

**Returns:**
boolean - un indicateur qui définit si les activités doivent être marquées comme critiques lors de la planification du projet.
### getRelationshipLagCalendar() {#getRelationshipLagCalendar--}
```
public final int getRelationshipLagCalendar()
```


Obtient une option qui définit quel calendrier utiliser pour planifier le retard de relation dans les projets Primavera.

**Returns:**
int - une option qui définit quel calendrier utiliser pour la planification du retard de relation dans les projets Primavera
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Obtient le nom court du projet (ID du projet).

**Returns:**
java.lang.String - nom court du projet (ID du projet).
### getUseExpectedFinishDates() {#getUseExpectedFinishDates--}
```
public final boolean getUseExpectedFinishDates()
```


Obtient un indicateur qui définit si les dates de fin d'activité doivent être planifiées comme les dates de fin prévues.

**Returns:**
boolean - un indicateur qui définit si les dates de fin d'activité doivent être planifiées comme les dates de fin attendues.
