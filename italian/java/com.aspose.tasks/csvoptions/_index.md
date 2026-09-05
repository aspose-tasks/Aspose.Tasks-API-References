---
title: "CsvOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Consente di specificare opzioni aggiuntive durante il salvataggio del progetto in CSV."
type: docs
weight: 56
url: /it/java/com.aspose.tasks/csvoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class CsvOptions extends SimpleSaveOptions
```

Consente di specificare opzioni aggiuntive durante il salvataggio del progetto in CSV.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [CsvOptions()](#CsvOptions--) | Inizializza una nuova istanza della classe [CsvOptions](../../com.aspose/tasks/csvoptions) che può essere usata per salvare il progetto in formato CSV. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getDataCategory()](#getDataCategory--) | Ottiene una categoria di dati da salvare. |
| [getEncoding()](#getEncoding--) | Ottiene una codifica per salvare il CSV. |
| [getIncludeHeaders()](#getIncludeHeaders--) | Ottiene un valore che indica se includere le intestazioni o meno (il valore predefinito è TRUE). |
| [getTextDelimiter()](#getTextDelimiter--) | Ottiene un delimitatore di testo. |
| [getView()](#getView--) | Ottiene un elenco delle colonne di visualizzazione ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) da salvare in formato XLSX. |
| [setDataCategory(int value)](#setDataCategory-int-) | Imposta una categoria di dati da salvare. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Imposta una codifica con cui salvare il CSV. |
| [setIncludeHeaders(boolean value)](#setIncludeHeaders-boolean-) | Imposta un valore che indica se includere le intestazioni o meno (il valore predefinito è TRUE). |
| [setTextDelimiter(int value)](#setTextDelimiter-int-) | Imposta un delimitatore di testo. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Imposta un elenco delle colonne di visualizzazione ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) da salvare in formato XLSX. |
### CsvOptions() {#CsvOptions--}
```
public CsvOptions()
```


Inizializza una nuova istanza della classe [CsvOptions](../../com.aspose/tasks/csvoptions) che può essere usata per salvare il progetto in formato CSV.

### getDataCategory() {#getDataCategory--}
```
public final int getDataCategory()
```


Ottiene una categoria di dati da salvare.

**Returns:**
int - una categoria di dati da salvare.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Ottiene una codifica per salvare il CSV.

**Returns:**
java.nio.charset.Charset - una codifica con cui salvare il CSV.
### getIncludeHeaders() {#getIncludeHeaders--}
```
public final boolean getIncludeHeaders()
```


Ottiene un valore che indica se includere le intestazioni o meno (il valore predefinito è TRUE).

**Returns:**
boolean - un valore che indica se includere le intestazioni o meno (il valore predefinito è TRUE).
### getTextDelimiter() {#getTextDelimiter--}
```
public final int getTextDelimiter()
```


Ottiene un delimitatore di testo.

**Returns:**
int - un delimitatore di testo.
### getView() {#getView--}
```
public final ProjectView getView()
```


Ottiene un elenco delle colonne di visualizzazione ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) da salvare in formato XLSX. Se non impostato, vengono salvate le colonne predefinite.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setDataCategory(int value) {#setDataCategory-int-}
```
public final void setDataCategory(int value)
```


Imposta una categoria di dati da salvare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | una categoria di dati da salvare. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Imposta una codifica con cui salvare il CSV.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.nio.charset.Charset | una codifica con cui salvare il CSV. |

### setIncludeHeaders(boolean value) {#setIncludeHeaders-boolean-}
```
public final void setIncludeHeaders(boolean value)
```


Imposta un valore che indica se includere le intestazioni o meno (il valore predefinito è TRUE).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se includere le intestazioni o meno (il valore predefinito è TRUE). |

### setTextDelimiter(int value) {#setTextDelimiter-int-}
```
public final void setTextDelimiter(int value)
```


Imposta un delimitatore di testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un delimitatore di testo. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Imposta un elenco delle colonne di visualizzazione ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) da salvare in formato XLSX. Se non impostato, vengono salvate le colonne predefinite.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | un elenco delle colonne di visualizzazione ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) da salvare in formato XLSX. |

