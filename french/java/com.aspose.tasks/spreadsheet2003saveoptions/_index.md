---
title: "Spreadsheet2003SaveOptions"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Permet de spécifier des options supplémentaires lors du rendu des pages de projet vers Spreadsheet2003."
type: docs
weight: 280
url: /fr/java/com.aspose.tasks/spreadsheet2003saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class Spreadsheet2003SaveOptions extends SimpleSaveOptions
```

Permet de spécifier des options supplémentaires lors du rendu des pages de projet vers Spreadsheet2003.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Spreadsheet2003SaveOptions()](#Spreadsheet2003SaveOptions--) | Initialise une nouvelle instance de la classe [Spreadsheet2003SaveOptions](../../com.aspose.tasks/spreadsheet2003saveoptions). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | Obtient une liste des colonnes d'affichage des affectations à rendre ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getResourceView()](#getResourceView--) | Obtient une liste des colonnes d'affichage des ressources à rendre ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [getView()](#getView--) | Obtient une liste des colonnes d'affichage ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) à enregistrer. |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | Définit une liste des colonnes d'affichage des affectations à rendre ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | Définit une liste des colonnes d'affichage des ressources à rendre ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Définit une liste des colonnes d'affichage ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) à enregistrer. |
### Spreadsheet2003SaveOptions() {#Spreadsheet2003SaveOptions--}
```
public Spreadsheet2003SaveOptions()
```


Initialise une nouvelle instance de la classe [Spreadsheet2003SaveOptions](../../com.aspose.tasks/spreadsheet2003saveoptions).

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


Obtient une liste des colonnes d'affichage des affectations à rendre ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getResourceView() {#getResourceView--}
```
public final ProjectView getResourceView()
```


Obtient une liste des colonnes d'affichage des ressources à rendre ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).
### getView() {#getView--}
```
public final ProjectView getView()
```


Obtient une liste des colonnes d'affichage ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) à enregistrer. Si non défini, les colonnes par défaut sont enregistrées.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


Définit une liste des colonnes d'affichage des affectations à rendre ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | une liste des colonnes d'affichage des affectations à rendre ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

### setResourceView(ProjectView value) {#setResourceView-com.aspose.tasks.ProjectView-}
```
public final void setResourceView(ProjectView value)
```


Définit une liste des colonnes d'affichage des ressources à rendre ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | une liste des colonnes d'affichage des ressources à rendre ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Définit une liste des colonnes d'affichage ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) à enregistrer. Si non défini, les colonnes par défaut sont enregistrées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | une liste des colonnes d'affichage ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) à enregistrer. |

