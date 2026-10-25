---
title: "ProjectView"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Classe de vue des projets"
type: docs
weight: 228
url: /fr/java/com.aspose.tasks/projectview/
---

**Inheritance:**
java.lang.Object
```
public class ProjectView
```

Classe de vue du projet
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ProjectView(Iterable&lt;ViewColumn&gt; columns)](#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--) | Initialise une nouvelle instance de la classe [ProjectView](../../com.aspose.tasks/projectview). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getColumns()](#getColumns--) | Obtient les colonnes de la vue du projet. |
| [getDefaultAssignmentView()](#getDefaultAssignmentView--) | Inclut les colonnes Uid, nom de tâche, nom de ressource, travail et durée d'affectation. |
| [getDefaultGanttChartView()](#getDefaultGanttChartView--) | Inclut id, indicateurs, nom, durée, début et fin des colonnes de tâche. |
| [getDefaultResourceSheetView()](#getDefaultResourceSheetView--) | Inclut Uid, nom de la ressource, type, libellé du matériau, initiales, groupe, unités max, tarif standard, tarif des heures supplémentaires, coût par utilisation, accumulé à, calendrier de base et colonnes de code de ressource. |
| [getDefaultResourceUsageView()](#getDefaultResourceUsageView--) | Inclut Uid, nom, début, fin et colonnes de ressource de travail. |
| [getDefaultTaskSheetView()](#getDefaultTaskSheetView--) | Inclut id, indicateurs, nom, durée, début, fin, prédécesseurs et noms de ressources des colonnes de tâche. |
### ProjectView(Iterable&lt;ViewColumn&gt; columns) {#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--}
```
public ProjectView(Iterable<ViewColumn> columns)
```


Initialise une nouvelle instance de la classe [ProjectView](../../com.aspose.tasks/projectview).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| colonnes | java.lang.Iterable&lt;com.aspose.tasks.ViewColumn&gt; | Une liste des colonnes de vue. |

### getColumns() {#getColumns--}
```
public final List<ViewColumn> getColumns()
```


Obtient les colonnes de la vue du projet.

**Returns:**
java.util.List&lt;com.aspose.tasks.ViewColumn&gt; - les colonnes de vue du projet.
### getDefaultAssignmentView() {#getDefaultAssignmentView--}
```
public static ProjectView getDefaultAssignmentView()
```


Inclut les colonnes Uid, nom de tâche, nom de ressource, travail et durée d'affectation.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn).
### getDefaultGanttChartView() {#getDefaultGanttChartView--}
```
public static ProjectView getDefaultGanttChartView()
```


Inclut id, indicateurs, nom, durée, début et fin des colonnes de tâche.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
### getDefaultResourceSheetView() {#getDefaultResourceSheetView--}
```
public static ProjectView getDefaultResourceSheetView()
```


Inclut Uid, nom de la ressource, type, libellé du matériau, initiales, groupe, unités max, tarif standard, tarif des heures supplémentaires, coût par utilisation, accumulé à, calendrier de base et colonnes de code de ressource.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultResourceUsageView() {#getDefaultResourceUsageView--}
```
public static ProjectView getDefaultResourceUsageView()
```


Inclut Uid, nom, début, fin et colonnes de ressource de travail.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultTaskSheetView() {#getDefaultTaskSheetView--}
```
public static ProjectView getDefaultTaskSheetView()
```


Inclut id, indicateurs, nom, durée, début, fin, prédécesseurs et noms de ressources des colonnes de tâche.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
