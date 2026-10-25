---
title: "AssignmentViewColumn"
second_title: "Aspose.Tasks for Java API Reference"
description: "Classe di visualizzazione dei progetti."
type: docs
weight: 19
url: /it/java/com.aspose.tasks/assignmentviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public class AssignmentViewColumn extends ViewColumn
```

Classe di visualizzazione del progetto.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)](#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-) | Inizializza una nuova istanza della classe AssignmentViewColumn. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getColumnText(ResourceAssignment assignment)](#getColumnText-com.aspose.tasks.ResourceAssignment-) | Converte l'assegnazione corrente della risorsa in testo della colonna. |
| [getField()](#getField--) | Restituisce il campo della colonna. |
| [setField(int value)](#setField-int-) | Imposta il campo della colonna. |
### AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter) {#AssignmentViewColumn-java.lang.String-int-com.aspose.tasks.AssignmentToColumnTextConverter-}
```
public AssignmentViewColumn(String name, int width, AssignmentToColumnTextConverter converter)
```


Inizializza una nuova istanza della classe AssignmentViewColumn.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Nome della colonna. |
| width | int | Larghezza della colonna in pixel. |
| converter | [AssignmentToColumnTextConverter](../../com.aspose.tasks/assignmenttocolumntextconverter) | Convertitore di dati di assegnazione in testo della colonna. |

### getColumnText(ResourceAssignment assignment) {#getColumnText-com.aspose.tasks.ResourceAssignment-}
```
public String getColumnText(ResourceAssignment assignment)
```


Converte l'assegnazione corrente della risorsa in testo della colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| assignment | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Assegnazione corrente. |

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

