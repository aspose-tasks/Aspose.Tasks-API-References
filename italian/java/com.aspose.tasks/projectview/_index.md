---
title: "ProjectView"
second_title: "Aspose.Tasks for Java API Reference"
description: "Classe di visualizzazione dei progetti"
type: docs
weight: 228
url: /it/java/com.aspose.tasks/projectview/
---

**Inheritance:**
java.lang.Object
```
public class ProjectView
```

Classe della vista del progetto
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ProjectView(Iterable&lt;ViewColumn&gt; columns)](#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--) | Inizializza una nuova istanza della classe [ProjectView](../../com.aspose.tasks/projectview). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getColumns()](#getColumns--) | Ottiene le colonne della vista progetto. |
| [getDefaultAssignmentView()](#getDefaultAssignmentView--) | Include le colonne Uid, nome attività, nome risorsa, lavoro e durata dell'assegnazione. |
| [getDefaultGanttChartView()](#getDefaultGanttChartView--) | Include id, indicatori, nome, durata, inizio e fine colonne delle attività. |
| [getDefaultResourceSheetView()](#getDefaultResourceSheetView--) | Include Uid, nome risorsa, tipo, etichetta materiale, iniziali, gruppo, unità massime, tariffa standard, tariffa straordinaria, costo per utilizzo, accumulo a, calendario base e colonne codice risorsa. |
| [getDefaultResourceUsageView()](#getDefaultResourceUsageView--) | Include Uid, nome, inizio, fine e colonne risorsa di lavoro. |
| [getDefaultTaskSheetView()](#getDefaultTaskSheetView--) | Include id, indicatori, nome, durata, inizio, fine, predecessori e nomi risorsa colonne delle attività. |
### ProjectView(Iterable&lt;ViewColumn&gt; columns) {#ProjectView-java.lang.Iterable-com.aspose.tasks.ViewColumn--}
```
public ProjectView(Iterable<ViewColumn> columns)
```


Inizializza una nuova istanza della classe [ProjectView](../../com.aspose.tasks/projectview).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonne | java.lang.Iterable&lt;com.aspose.tasks.ViewColumn&gt; | Un elenco delle colonne di visualizzazione. |

### getColumns() {#getColumns--}
```
public final List<ViewColumn> getColumns()
```


Ottiene le colonne della vista progetto.

**Returns:**
java.util.List&lt;com.aspose.tasks.ViewColumn&gt; - le colonne di visualizzazione del progetto.
### getDefaultAssignmentView() {#getDefaultAssignmentView--}
```
public static ProjectView getDefaultAssignmentView()
```


Include le colonne Uid, nome attività, nome risorsa, lavoro e durata dell'assegnazione.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn).
### getDefaultGanttChartView() {#getDefaultGanttChartView--}
```
public static ProjectView getDefaultGanttChartView()
```


Include id, indicatori, nome, durata, inizio e fine colonne delle attività.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
### getDefaultResourceSheetView() {#getDefaultResourceSheetView--}
```
public static ProjectView getDefaultResourceSheetView()
```


Include Uid, nome risorsa, tipo, etichetta materiale, iniziali, gruppo, unità massime, tariffa standard, tariffa straordinaria, costo per utilizzo, accumulo a, calendario base e colonne codice risorsa.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultResourceUsageView() {#getDefaultResourceUsageView--}
```
public static ProjectView getDefaultResourceUsageView()
```


Include Uid, nome, inizio, fine e colonne risorsa di lavoro.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).
### getDefaultTaskSheetView() {#getDefaultTaskSheetView--}
```
public static ProjectView getDefaultTaskSheetView()
```


Include id, indicatori, nome, durata, inizio, fine, predecessori e nomi risorsa colonne delle attività.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a view which contains a list of [GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn).
