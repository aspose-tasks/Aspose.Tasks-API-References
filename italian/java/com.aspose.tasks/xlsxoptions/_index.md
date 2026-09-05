---
title: "XlsxOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in XLSX."
type: docs
weight: 368
url: /it/java/com.aspose.tasks/xlsxoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class XlsxOptions extends SimpleSaveOptions
```

Consente di specificare opzioni aggiuntive durante il rendering delle pagine del progetto in XLSX.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [XlsxOptions()](#XlsxOptions--) | Inizializza una nuova istanza della classe [XlsxOptions](../../com.aspose.tasks/xlsxoptions) che può essere usata per salvare il progetto in formato XLSX. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getAssignmentView()](#getAssignmentView--) | Ottiene un elenco delle colonne di visualizzazione delle assegnazioni da visualizzare ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [getEncoding()](#getEncoding--) | Ottiene la codifica del file XLSX risultante. |
| [getResourceView()](#getResourceView--) | Ottiene un elenco delle colonne di visualizzazione delle risorse da visualizzare ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [getView()](#getView--) | Ottiene un elenco delle colonne di visualizzazione ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) da salvare in formato XLSX. |
| [setAssignmentView(ProjectView value)](#setAssignmentView-com.aspose.tasks.ProjectView-) | Imposta un elenco delle colonne di visualizzazione delle assegnazioni da visualizzare ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Imposta la codifica del file XLSX risultante. |
| [setResourceView(ProjectView value)](#setResourceView-com.aspose.tasks.ProjectView-) | Imposta un elenco delle colonne di visualizzazione delle risorse da visualizzare ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Imposta un elenco delle colonne di visualizzazione ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) da salvare in formato XLSX. |
### XlsxOptions() {#XlsxOptions--}
```
public XlsxOptions()
```


Inizializza una nuova istanza della classe [XlsxOptions](../../com.aspose.tasks/xlsxoptions) che può essere usata per salvare il progetto in formato XLSX.

### getAssignmentView() {#getAssignmentView--}
```
public final ProjectView getAssignmentView()
```


Ottiene un elenco delle colonne di visualizzazione delle assegnazioni da visualizzare ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the assignments view columns to render ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Ottiene la codifica del file XLSX risultante. Il valore predefinito è java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Returns:**
java.nio.charset.Charset - la codifica del file XLSX risultante.
### getResourceView() {#getResourceView--}
```
public final ProjectView getResourceView()
```


Ottiene un elenco delle colonne di visualizzazione delle risorse da visualizzare ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the resource view columns to render ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).
### getView() {#getView--}
```
public final ProjectView getView()
```


Ottiene un elenco delle colonne di visualizzazione ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) da salvare in formato XLSX. Se non impostato, vengono salvate le colonne predefinite.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setAssignmentView(ProjectView value) {#setAssignmentView-com.aspose.tasks.ProjectView-}
```
public final void setAssignmentView(ProjectView value)
```


Imposta un elenco delle colonne di visualizzazione delle assegnazioni da visualizzare ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | un elenco delle colonne di visualizzazione delle assegnazioni da visualizzare ([AssignmentViewColumn](../../com.aspose.tasks/assignmentviewcolumn)). |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Imposta la codifica del file XLSX risultante. Il valore predefinito è java.nio.charset.StandardCharsets\#UTF\_8.UTF\_8.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.nio.charset.Charset | la codifica del file XLSX risultante. |

### setResourceView(ProjectView value) {#setResourceView-com.aspose.tasks.ProjectView-}
```
public final void setResourceView(ProjectView value)
```


Imposta un elenco delle colonne di visualizzazione delle risorse da visualizzare ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | un elenco delle colonne di visualizzazione delle risorse da visualizzare ([ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn)). |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Imposta un elenco delle colonne di visualizzazione ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) da salvare in formato XLSX. Se non impostato, vengono salvate le colonne predefinite.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | un elenco delle colonne di visualizzazione ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) da salvare in formato XLSX. |

