---
title: "ProjectView"
second_title: "Aspose.Tasks for Java API Reference"
description: "Projektansicht‑Klasse"
type: docs
weight: 228
url: /de/java/com.aspose.tasks/projectview/
---

**Inheritance:**
java.lang.Object
```
public class ProjectView
```

Projekt‑Ansichtsklasse
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ProjectView(Iterable&lt;ViewColumn&gt; columns)](#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--) | Initialisiert eine neue Instanz der Klasse [ProjectView](../../com.aspose.tasks/projectview). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getColumns()](#getColumns--) | Ruft die Spalten der Projektansicht ab. |
| [getDefaultAssignmentView()](#getDefaultAssignmentView--) | Enthält Uid, Aufgabenname, Ressourcenname, Arbeits- und Dauereinsatzspalten. |
| [getDefaultGanttChartView()](#getDefaultGanttChartView--) | Enthält id, Indikatoren, Name, Dauer, Start- und Endaufgabenspalten. |
| [getDefaultResourceSheetView()](#getDefaultResourceSheetView--) | Enthält Uid, Ressourcenname, Typ, Materialbezeichnung, Initialen, Gruppe, maximale Einheiten, Standardrate, Überstundensatz, Kosten pro Nutzung, Anhäufung bei, Basiskalender und Code-Ressourcenspalten. |
| [getDefaultResourceUsageView()](#getDefaultResourceUsageView--) | Enthält Uid, Name, Start, Ende und Arbeitsressourcenspalten. |
| [getDefaultTaskSheetView()](#getDefaultTaskSheetView--) | Enthält id, Indikatoren, Name, Dauer, Start, Ende, Vorgänger und Ressourcennamen Aufgabenspalten. |
### ProjectView(Iterable&lt;ViewColumn&gt; columns) {#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--}
```
public ProjectView(Iterable<ViewColumn> columns)
```


Initialisiert eine neue Instanz der Klasse [ProjectView](../../com.aspose.tasks/projectview).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalten | java.lang.Iterable&lt;com.aspose.tasks.ViewColumn&gt; | Eine Liste der Ansichtsspalten. |

### getColumns() {#getColumns--}
```
public final List<ViewColumn> getColumns()
```


Ruft die Spalten der Projektansicht ab.

**Returns:**
java.util.List&lt;com.aspose.tasks.ViewColumn&gt; - die Projektansichtsspalten.
### getDefaultAssignmentView() {#getDefaultAssignmentView--}
```
public static ProjectView getDefaultAssignmentView()
```


Enthält Uid, Aufgabenname, Ressourcenname, Arbeits- und Dauereinsatzspalten.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn).
### getDefaultGanttChartView() {#getDefaultGanttChartView--}
```
public static ProjectView getDefaultGanttChartView()
```


Enthält id, Indikatoren, Name, Dauer, Start- und Endaufgabenspalten.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
### getDefaultResourceSheetView() {#getDefaultResourceSheetView--}
```
public static ProjectView getDefaultResourceSheetView()
```


Enthält Uid, Ressourcenname, Typ, Materialbezeichnung, Initialen, Gruppe, maximale Einheiten, Standardrate, Überstundensatz, Kosten pro Nutzung, Anhäufung bei, Basiskalender und Code-Ressourcenspalten.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultResourceUsageView() {#getDefaultResourceUsageView--}
```
public static ProjectView getDefaultResourceUsageView()
```


Enthält Uid, Name, Start, Ende und Arbeitsressourcenspalten.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultTaskSheetView() {#getDefaultTaskSheetView--}
```
public static ProjectView getDefaultTaskSheetView()
```


Enthält id, Indikatoren, Name, Dauer, Start, Ende, Vorgänger und Ressourcennamen Aufgabenspalten.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
