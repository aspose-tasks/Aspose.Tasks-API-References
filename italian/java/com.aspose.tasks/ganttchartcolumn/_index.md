---
title: "GanttChartColumn"
second_title: "Aspose.Tasks for Java API Reference"
description: "Classe di visualizzazione dei progetti"
type: docs
weight: 111
url: /it/java/com.aspose.tasks/ganttchartcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class GanttChartColumn extends ViewColumn
```

Classe della vista del progetto
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-) | Inizializza una nuova istanza della classe GanttChartColumn. |
| [GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)](#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-) | Inizializza una nuova istanza della classe GanttChartColumn. |
| [GanttChartColumn(int width, int field)](#GanttChartColumn-int-int-) | Inizializza una nuova istanza della classe GanttChartColumn. |
| [GanttChartColumn(String name, int width, int field)](#GanttChartColumn-java.lang.String-int-int-) | Inizializza una nuova istanza della classe GanttChartColumn. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getColumnText(Task task)](#getColumnText-com.aspose.tasks.Task-) | Converte l'attività corrente in testo di colonna. |
| [getField()](#getField--) | Restituisce il campo della colonna. |
| [setField(int value)](#setField-int-) | Imposta il campo della colonna. |
### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-int-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter, int field)
```


Inizializza una nuova istanza della classe GanttChartColumn.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Nome della colonna. |
| width | int | Larghezza della colonna in pixel. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Convertitore da dati dell'attività a testo di colonna. |
| campo | int | Campo della colonna. |

### GanttChartColumn(String name, int width, TaskToColumnTextConverter converter) {#GanttChartColumn-java.lang.String-int-com.aspose.tasks.TaskToColumnTextConverter-}
```
public GanttChartColumn(String name, int width, TaskToColumnTextConverter converter)
```


Inizializza una nuova istanza della classe GanttChartColumn.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Nome della colonna. |
| width | int | Larghezza della colonna in pixel. |
| converter | [TaskToColumnTextConverter](../../com.aspose.tasks/tasktocolumntextconverter) | Convertitore da dati dell'attività a testo di colonna. |

### GanttChartColumn(int width, int field) {#GanttChartColumn-int-int-}
```
public GanttChartColumn(int width, int field)
```


Inizializza una nuova istanza della classe GanttChartColumn.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| width | int | Larghezza della colonna in pixel. |
| campo | int | Campo della colonna. |

### GanttChartColumn(String name, int width, int field) {#GanttChartColumn-java.lang.String-int-int-}
```
public GanttChartColumn(String name, int width, int field)
```


Inizializza una nuova istanza della classe GanttChartColumn.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Nome della colonna. |
| width | int | Larghezza della colonna in pixel. |
| campo | int | Campo della colonna. |

### getColumnText(Task task) {#getColumnText-com.aspose.tasks.Task-}
```
public final String getColumnText(Task task)
```


Converte l'attività corrente in testo di colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Attività corrente. |

**Returns:**
java.lang.String - Il testo della colonna.
### getField() {#getField--}
```
public int getField()
```


Restituisce il campo della colonna. `Field`.

**Returns:**
int - valore del campo della colonna.
### setField(int value) {#setField-int-}
```
public void setField(int value)
```


Imposta il campo della colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | valore del campo della colonna. |

