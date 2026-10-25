---
title: "XlsxOptions"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Permet de spécifier des options supplémentaires lors du rendu des pages de projet en XLSX."
type: docs
weight: 368
url: /fr/java/com.aspose.tasks/xlsxoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class XlsxOptions extends SimpleSaveOptions
```

Permet de spécifier des options supplémentaires lors du rendu des pages de projet en XLSX.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [XlsxOptions()](#XlsxOptions--) | Initialise une nouvelle instance de la classe [XlsxOptions](../../com.aspose.tasks/xlsxoptions) qui peut être utilisée pour enregistrer le projet au format XLSX. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | Obtient une liste des colonnes d'affichage des affectations à rendre ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getEncoding()](#getEncoding--) | Obtient l'encodage du fichier XLSX résultant. |
| [getResourceView()](#getResourceView--) | Obtient une liste des colonnes d'affichage des ressources à rendre ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [getView()](#getView--) | Obtient une liste des colonnes de vue ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) à enregistrer au format XLSX. |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | Définit une liste des colonnes d'affichage des affectations à rendre ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Définit l'encodage du fichier XLSX résultant. |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | Définit une liste des colonnes d'affichage des ressources à rendre ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Définit une liste des colonnes de vue ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) à enregistrer au format XLSX. |
### XlsxOptions() {#XlsxOptions--}
```
public XlsxOptions()
```


Initialise une nouvelle instance de la classe [XlsxOptions](../../com.aspose.tasks/xlsxoptions) qui peut être utilisée pour enregistrer le projet au format XLSX.

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


Obtient une liste des colonnes d'affichage des affectations à rendre ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Obtient l'encodage du fichier XLSX résultant. La valeur par défaut est java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Returns:**
java.nio.charset.Charset - l'encodage du fichier XLSX résultant.
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


Obtient une liste des colonnes de vue ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) à enregistrer au format XLSX. Si non défini, les colonnes par défaut sont enregistrées.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


Définit une liste des colonnes d'affichage des affectations à rendre ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | une liste des colonnes d'affichage des affectations à rendre ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Définit l'encodage du fichier XLSX résultant. La valeur par défaut est java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.nio.charset.Charset | l'encodage du fichier XLSX résultant. |

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


Définit une liste des colonnes de vue ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) à enregistrer au format XLSX. Si non défini, les colonnes par défaut sont enregistrées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | une liste des colonnes de vue ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) à enregistrer au format XLSX. |

