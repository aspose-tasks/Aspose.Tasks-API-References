---
title: "ProjectView"
second_title: "Aspose.Tasks for Java API-referens"
description: "Projektvy-klass"
type: docs
weight: 228
url: /sv/java/com.aspose.tasks/projectview/
---

**Inheritance:**
java.lang.Object
```
public class ProjectView
```

Projektets vyklass
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ProjectView(Iterable&lt;ViewColumn&gt; columns)](#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--) | Initierar en ny instans av klassen [ProjectView](../../com.aspose.tasks/projectview). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getColumns()](#getColumns--) | Hämtar kolumnerna för projektvyn. |
| [getDefaultAssignmentView()](#getDefaultAssignmentView--) | Inkluderar Uid, uppgiftsnamn, resursnamn, arbets- och varaktighetstilldelningskolumner. |
| [getDefaultGanttChartView()](#getDefaultGanttChartView--) | Inkluderar id, indikatorer, namn, varaktighet, start- och slutuppgiftskolumner. |
| [getDefaultResourceSheetView()](#getDefaultResourceSheetView--) | Inkluderar Uid, resursnamn, typ, materialetikett, initialer, grupp, maxenheter, standardpris, övertidspris, kostnad per användning, ackumuleras vid, grundkalender och kodresurskolumner. |
| [getDefaultResourceUsageView()](#getDefaultResourceUsageView--) | Inkluderar Uid, namn, start, slut och arbetsresurskolumner. |
| [getDefaultTaskSheetView()](#getDefaultTaskSheetView--) | Inkluderar id, indikatorer, namn, varaktighet, start, slut, föregångare och resursnamn uppgiftskolumner. |
### ProjectView(Iterable&lt;ViewColumn&gt; columns) {#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--}
```
public ProjectView(Iterable<ViewColumn> columns)
```


Initierar en ny instans av klassen [ProjectView](../../com.aspose.tasks/projectview).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumner | java.lang.Iterable&lt;com.aspose.tasks.ViewColumn&gt; | En lista över vykolumnerna. |

### getColumns() {#getColumns--}
```
public final List<ViewColumn> getColumns()
```


Hämtar kolumnerna för projektvyn.

**Returns:**
java.util.List&lt;com.aspose.tasks.ViewColumn&gt; - projektvykolumnerna.
### getDefaultAssignmentView() {#getDefaultAssignmentView--}
```
public static ProjectView getDefaultAssignmentView()
```


Inkluderar Uid, uppgiftsnamn, resursnamn, arbets- och varaktighetstilldelningskolumner.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn).
### getDefaultGanttChartView() {#getDefaultGanttChartView--}
```
public static ProjectView getDefaultGanttChartView()
```


Inkluderar id, indikatorer, namn, varaktighet, start- och slutuppgiftskolumner.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
### getDefaultResourceSheetView() {#getDefaultResourceSheetView--}
```
public static ProjectView getDefaultResourceSheetView()
```


Inkluderar Uid, resursnamn, typ, materialetikett, initialer, grupp, maxenheter, standardpris, övertidspris, kostnad per användning, ackumuleras vid, grundkalender och kodresurskolumner.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultResourceUsageView() {#getDefaultResourceUsageView--}
```
public static ProjectView getDefaultResourceUsageView()
```


Inkluderar Uid, namn, start, slut och arbetsresurskolumner.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultTaskSheetView() {#getDefaultTaskSheetView--}
```
public static ProjectView getDefaultTaskSheetView()
```


Inkluderar id, indikatorer, namn, varaktighet, start, slut, föregångare och resursnamn uppgiftskolumner.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
