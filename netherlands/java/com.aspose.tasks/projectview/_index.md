---
title: "ProjectView"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Projects view-klasse"
type: docs
weight: 228
url: /nl/java/com.aspose.tasks/projectview/
---

**Inheritance:**
java.lang.Object
```
public class ProjectView
```

Projectweergaveklasse
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ProjectView(Iterable&lt;ViewColumn&gt; columns)](#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--) | Initialiseert een nieuw exemplaar van de [ProjectView](../../com.aspose.tasks/projectview) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getColumns()](#getColumns--) | Haalt de kolommen van de projectweergave op. |
| [getDefaultAssignmentView()](#getDefaultAssignmentView--) | Bevat Uid, taaknaam, resource-naam, werk- en duurtoewijzingskolommen. |
| [getDefaultGanttChartView()](#getDefaultGanttChartView--) | Bevat id, indicatoren, naam, duur, start- en eindtaakkolommen. |
| [getDefaultResourceSheetView()](#getDefaultResourceSheetView--) | Bevat Uid, resource‑naam, type, materiaallabel, initialen, groep, maximale eenheden, standaardtarief, overurenttarief, kosten per gebruik, opbouw op, basis‑kalender en code‑resourcekolommen. |
| [getDefaultResourceUsageView()](#getDefaultResourceUsageView--) | Bevat Uid, naam, start, finish en werk‑resourcekolommen. |
| [getDefaultTaskSheetView()](#getDefaultTaskSheetView--) | Bevat id, indicatoren, naam, duur, start, finish, voorgangers en resource‑namen taakkolommen. |
### ProjectView(Iterable&lt;ViewColumn&gt; columns) {#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--}
```
public ProjectView(Iterable<ViewColumn> columns)
```


Initialiseert een nieuw exemplaar van de [ProjectView](../../com.aspose.tasks/projectview) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| kolommen | java.lang.Iterable&lt;com.aspose.tasks.ViewColumn&gt; | Een lijst van de weergavekolommen. |

### getColumns() {#getColumns--}
```
public final List<ViewColumn> getColumns()
```


Haalt de kolommen van de projectweergave op.

**Returns:**
java.util.List&lt;com.aspose.tasks.ViewColumn&gt; - de projectweergavekolommen.
### getDefaultAssignmentView() {#getDefaultAssignmentView--}
```
public static ProjectView getDefaultAssignmentView()
```


Bevat Uid, taaknaam, resource-naam, werk- en duurtoewijzingskolommen.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn).
### getDefaultGanttChartView() {#getDefaultGanttChartView--}
```
public static ProjectView getDefaultGanttChartView()
```


Bevat id, indicatoren, naam, duur, start- en eindtaakkolommen.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
### getDefaultResourceSheetView() {#getDefaultResourceSheetView--}
```
public static ProjectView getDefaultResourceSheetView()
```


Bevat Uid, resource‑naam, type, materiaallabel, initialen, groep, maximale eenheden, standaardtarief, overurenttarief, kosten per gebruik, opbouw op, basis‑kalender en code‑resourcekolommen.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultResourceUsageView() {#getDefaultResourceUsageView--}
```
public static ProjectView getDefaultResourceUsageView()
```


Bevat Uid, naam, start, finish en werk‑resourcekolommen.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultTaskSheetView() {#getDefaultTaskSheetView--}
```
public static ProjectView getDefaultTaskSheetView()
```


Bevat id, indicatoren, naam, duur, start, finish, voorgangers en resource‑namen taakkolommen.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
