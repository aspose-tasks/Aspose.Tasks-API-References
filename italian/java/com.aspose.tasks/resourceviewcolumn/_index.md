---
title: "ResourceViewColumn"
second_title: "Aspose.Tasks for Java API Reference"
description: "Classe di visualizzazione dei progetti utilizzata nella vista ResourceUsage e nella vista ResourceSheet."
type: docs
weight: 261
url: /it/java/com.aspose.tasks/resourceviewcolumn/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.ViewColumn](../../com.aspose.tasks/viewcolumn)
```
public final class ResourceViewColumn extends ViewColumn
```

Classe di vista del progetto utilizzata nella vista ResourceUsage e nella vista ResourceSheet.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-) | Inizializza una nuova istanza della classe [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
| [ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)](#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-) | Inizializza una nuova istanza della classe [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
| [ResourceViewColumn(int width, int field)](#ResourceViewColumn-int-int-) | Inizializza una nuova istanza della classe [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getColumnText(Resource resource)](#getColumnText-com.aspose.tasks.Resource-) | Converte la risorsa corrente nel testo della colonna. |
| [getField()](#getField--) | Restituisce il campo della colonna. |
| [setField(int value)](#setField-int-) | Imposta il campo della colonna. |
### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-int-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter, int field)
```


Inizializza una nuova istanza della classe [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Nome della colonna. |
| width | int | Larghezza della colonna in pixel. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Convertitore di dati della risorsa in testo della colonna. |
| campo | int | Campo della colonna. |

### ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter) {#ResourceViewColumn-java.lang.String-int-com.aspose.tasks.ResourceToColumnTextConverter-}
```
public ResourceViewColumn(String name, int width, ResourceToColumnTextConverter converter)
```


Inizializza una nuova istanza della classe [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Nome della colonna. |
| width | int | Larghezza della colonna in pixel. |
| converter | [ResourceToColumnTextConverter](../../com.aspose.tasks/resourcetocolumntextconverter) | Convertitore di dati della risorsa in testo della colonna. |

### ResourceViewColumn(int width, int field) {#ResourceViewColumn-int-int-}
```
public ResourceViewColumn(int width, int field)
```


Inizializza una nuova istanza della classe [ResourceViewColumn](../../com.aspose.tasks/resourceviewcolumn).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| width | int | Larghezza della colonna in pixel. |
| campo | int | Campo della colonna. |

### getColumnText(Resource resource) {#getColumnText-com.aspose.tasks.Resource-}
```
public final String getColumnText(Resource resource)
```


Converte la risorsa corrente nel testo della colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| resource | [Resource](../../com.aspose.tasks/resource) | Risorsa corrente. |

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

