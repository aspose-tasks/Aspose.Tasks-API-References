---
title: "OutlineValue"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un valore di outline."
type: docs
weight: 173
url: /it/java/com.aspose.tasks/outlinevalue/
---

**Inheritance:**
java.lang.Object
```
public class OutlineValue
```

Rappresenta un valore di outline.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [OutlineValue()](#OutlineValue--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getDescription()](#getDescription--) | Restituisce la descrizione di un valore di outline. |
| [getDurationValue()](#getDurationValue--) | Restituisce la durata se il Tipo è Durata. |
| [getParentValueId()](#getParentValueId--) | Restituisce l'Id di un nodo genitore di un codice outline. |
| [getType()](#getType--) | Restituisce il tipo di codice outline. |
| [getValue()](#getValue--) | Restituisce il valore effettivo. |
| [getValueGuid()](#getValueGuid--) | Restituisce un GUID che identifica questo valore tra gli altri nell'intero progetto. |
| [getValueId()](#getValueId--) | Restituisce l'Id univoco di un valore di codice outline all'interno di un progetto. |
| [isCollapsed()](#isCollapsed--) | Restituisce un valore che indica se il valore di outline è collassato o meno. |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | Imposta un valore che indica se il valore di outline è collassato o meno. |
| [setDescription(String value)](#setDescription-java.lang.String-) | Imposta la descrizione di un valore di outline. |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | Imposta la durata se il Tipo è Durata. |
| [setParentValueId(int value)](#setParentValueId-int-) | Imposta l'Id di un nodo genitore di un codice outline. |
| [setType(int value)](#setType-int-) | Imposta il tipo di codice outline. |
| [setValue(String value)](#setValue-java.lang.String-) | Imposta il valore effettivo. |
| [setValueId(int value)](#setValueId-int-) | Imposta l'Id univoco di un valore di codice outline all'interno di un progetto. |
### OutlineValue() {#OutlineValue--}
```
public OutlineValue()
```


### getDescription() {#getDescription--}
```
public final String getDescription()
```


Restituisce la descrizione di un valore di outline.

**Returns:**
java.lang.String - la descrizione di un valore di outline.
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


Restituisce la durata se il Tipo è Durata.

--------------------

Preferisci questa proprietà rispetto a `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)), quando devi impostare il valore per OutlineValues con tipo Duration.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration if Type is Duration.
### getParentValueId() {#getParentValueId--}
```
public final int getParentValueId()
```


Restituisce l'Id di un nodo genitore di un codice outline.

**Returns:**
int - l'Id di un nodo genitore di un codice outline.
### getType() {#getType--}
```
public final int getType()
```


Restituisce il tipo di codice outline.

**Returns:**
int - il tipo di codice outline.
### getValue() {#getValue--}
```
public final String getValue()
```


Restituisce il valore effettivo.

**Returns:**
java.lang.String - il valore effettivo.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


Restituisce un GUID che identifica questo valore tra gli altri nell'intero progetto.

**Returns:**
java.util.UUID - un GUID che identifica questo valore tra gli altri in tutto il progetto.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


Restituisce l'Id univoco di un valore di codice outline all'interno di un progetto.

**Returns:**
int - l'Id univoco di un valore di codice outline all'interno di un progetto.
### isCollapsed() {#isCollapsed--}
```
public final boolean isCollapsed()
```


Restituisce un valore che indica se il valore di outline è collassato o meno.

--------------------

Questa è una nuova proprietà per MS Project 2010.

**Returns:**
boolean - un valore che indica se il valore di outline è collassato o meno.
### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public final void setCollapsed(boolean value)
```


Imposta un valore che indica se il valore di outline è collassato o meno.

--------------------

Questa è una nuova proprietà per MS Project 2010.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se il valore della struttura è compresso o meno. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


Imposta la descrizione di un valore di outline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | la descrizione di un valore della struttura. |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


Imposta la durata se il Tipo è Durata.

--------------------

Preferisci questa proprietà rispetto a `Value`([getValue()](../../com.aspose.tasks/outlinevalue\#getValue--)/[setValue(String)](../../com.aspose.tasks/outlinevalue\#setValue-String-)), quando devi impostare il valore per OutlineValues con tipo Duration.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | la durata se il Tipo è Durata. |

### setParentValueId(int value) {#setParentValueId-int-}
```
public final void setParentValueId(int value)
```


Imposta l'Id di un nodo genitore di un codice outline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | l'Id di un nodo genitore di un codice della struttura. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Imposta il tipo di codice outline.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il tipo di codice della struttura. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


Imposta il valore effettivo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | il valore effettivo. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


Imposta l'Id univoco di un valore di codice outline all'interno di un progetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | l'Id univoco di un valore di codice della struttura all'interno di un progetto. |

