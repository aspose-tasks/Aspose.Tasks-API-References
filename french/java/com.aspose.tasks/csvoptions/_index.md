---
title: "CsvOptions"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Permet de spécifier des options supplémentaires lors de l'enregistrement du projet au format CSV."
type: docs
weight: 56
url: /fr/java/com.aspose.tasks/csvoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class CsvOptions extends SimpleSaveOptions
```

Permet de spécifier des options supplémentaires lors de l'enregistrement du projet au format CSV.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CsvOptions()](#CsvOptions--) | Initialise une nouvelle instance de la classe [CsvOptions](../../com.aspose/tasks/csvoptions) qui peut être utilisée pour enregistrer le projet au format CSV. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getDataCategory()](#getDataCategory--) | Obtient une catégorie de données à enregistrer. |
| [getEncoding()](#getEncoding--) | Obtient un encodage avec lequel enregistrer le CSV. |
| [getIncludeHeaders()](#getIncludeHeaders--) | Obtient une valeur indiquant s'il faut inclure les en-têtes ou non (la valeur par défaut est TRUE). |
| [getTextDelimiter()](#getTextDelimiter--) | Obtient un délimiteur de texte. |
| [getView()](#getView--) | Obtient une liste des colonnes de vue ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) à enregistrer au format XLSX. |
| [setDataCategory(int value)](#setDataCategory-int-) | Définit une catégorie de données à enregistrer. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Définit un encodage avec lequel enregistrer le CSV. |
| [setIncludeHeaders(boolean value)](#setIncludeHeaders-boolean-) | Définit une valeur indiquant s'il faut inclure les en-têtes ou non (la valeur par défaut est TRUE). |
| [setTextDelimiter(int value)](#setTextDelimiter-int-) | Définit un délimiteur de texte. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Définit une liste des colonnes de vue ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) à enregistrer au format XLSX. |
### CsvOptions() {#CsvOptions--}
```
public CsvOptions()
```


Initialise une nouvelle instance de la classe [CsvOptions](../../com.aspose/tasks/csvoptions) qui peut être utilisée pour enregistrer le projet au format CSV.

### getDataCategory() {#getDataCategory--}
```
public final int getDataCategory()
```


Obtient une catégorie de données à enregistrer.

**Returns:**
int - une catégorie de données à enregistrer.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Obtient un encodage avec lequel enregistrer le CSV.

**Returns:**
java.nio.charset.Charset - un encodage avec lequel enregistrer le CSV.
### getIncludeHeaders() {#getIncludeHeaders--}
```
public final boolean getIncludeHeaders()
```


Obtient une valeur indiquant s'il faut inclure les en-têtes ou non (la valeur par défaut est TRUE).

**Returns:**
boolean - une valeur indiquant s'il faut inclure les en-têtes ou non (la valeur par défaut est TRUE).
### getTextDelimiter() {#getTextDelimiter--}
```
public final int getTextDelimiter()
```


Obtient un délimiteur de texte.

**Returns:**
int - un délimiteur de texte.
### getView() {#getView--}
```
public final ProjectView getView()
```


Obtient une liste des colonnes de vue ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) à enregistrer au format XLSX. Si non défini, les colonnes par défaut sont enregistrées.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) to save to XLSX format.
### setDataCategory(int value) {#setDataCategory-int-}
```
public final void setDataCategory(int value)
```


Définit une catégorie de données à enregistrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une catégorie de données à enregistrer. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Définit un encodage avec lequel enregistrer le CSV.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.nio.charset.Charset | un encodage avec lequel enregistrer le CSV. |

### setIncludeHeaders(boolean value) {#setIncludeHeaders-boolean-}
```
public final void setIncludeHeaders(boolean value)
```


Définit une valeur indiquant s'il faut inclure les en-têtes ou non (la valeur par défaut est TRUE).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut inclure les en-têtes ou non (la valeur par défaut est TRUE). |

### setTextDelimiter(int value) {#setTextDelimiter-int-}
```
public final void setTextDelimiter(int value)
```


Définit un délimiteur de texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un délimiteur de texte. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Définit une liste des colonnes de vue ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) à enregistrer au format XLSX. Si non défini, les colonnes par défaut sont enregistrées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | une liste des colonnes de vue ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)) à enregistrer au format XLSX. |

