---
title: "Valore"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un valore in un elenco di valori."
type: docs
weight: 333
url: /it/java/com.aspose.tasks/value/
---

**Inheritance:**
java.lang.Object
```
public class Value
```

Rappresenta un valore in un elenco di valori.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Value()](#Value--) | Inizializza una nuova istanza della classe [Value](../../com.aspose/tasks/value). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getDateValue()](#getDateValue--) | Restituisce il valore effettivo se può essere rappresentato come DateTime. |
| [getDescription()](#getDescription--) | Restituisce la descrizione di un valore. |
| [getDuration()](#getDuration--) | Restituisce il valore effettivo utilizzato per rappresentare la Durata. |
| [getId()](#getId--) | Restituisce l'identificatore univoco di un valore nell'intero progetto. |
| [getNumericValue()](#getNumericValue--) | Restituisce il valore effettivo utilizzato per rappresentare un valore numerico o di costo. |
| [getPhonetic()](#getPhonetic--) | Restituisce le informazioni fonetiche sul nome del campo personalizzato. |
| [getStringValue()](#getStringValue--) | Restituisce il valore effettivo utilizzato per rappresentare una stringa di testo. |
| [getVal()](#getVal--) | Restituisce il valore effettivo nella rappresentazione interna. |
| [getValueGuid()](#getValueGuid--) | Restituisce un GUID che identifica questo valore tra gli altri nell'intero progetto. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Imposta il valore effettivo se può essere rappresentato come DateTime. |
| [setDescription(String value)](#setDescription-java.lang.String-) | Imposta la descrizione di un valore. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Imposta il valore effettivo utilizzato per rappresentare la Durata. |
| [setId(int value)](#setId-int-) | Imposta l'identificatore univoco di un valore nell'intero progetto. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Imposta il valore effettivo utilizzato per rappresentare un valore numerico o di costo. |
| [setPhonetic(String value)](#setPhonetic-java.lang.String-) | Imposta le informazioni fonetiche sul nome del campo personalizzato. |
| [setStringValue(String value)](#setStringValue-java.lang.String-) | Imposta il valore effettivo utilizzato per rappresentare una stringa di testo. |
| [setVal(String value)](#setVal-java.lang.String-) | Imposta il valore effettivo nella rappresentazione interna. |
### Value() {#Value--}
```
public Value()
```


Inizializza una nuova istanza della classe [Value](../../com.aspose/tasks/value).

### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Restituisce il valore effettivo se può essere rappresentato come DateTime. Il valore predefinito è DateTime\#MinValue.MinValue.

--------------------

Preferisci questa proprietà rispetto a `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), quando devi impostare il valore DateTime.

**Returns:**
java.util.Date - il valore effettivo se può essere rappresentato come DateTime.
### getDescription() {#getDescription--}
```
public final String getDescription()
```


Restituisce la descrizione di un valore.

**Returns:**
java.lang.String - la descrizione di un valore.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Restituisce il valore effettivo utilizzato per rappresentare la Durata.

--------------------

Preferisci questa proprietà rispetto a `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), quando devi impostare il valore Duration.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the actual value which is used to represent Duration.
### getId() {#getId--}
```
public final int getId()
```


Restituisce l'identificatore univoco di un valore nell'intero progetto.

È importante non avere gli stessi identificatori per diverse istanze di [Value](../../com.aspose.tasks/value).

Il valore minimo di `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) è `1`.

**Returns:**
int - l'identificatore univoco di un valore in tutto il progetto.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Restituisce il valore effettivo utilizzato per rappresentare un valore numerico o di costo.

--------------------

Preferisci questa proprietà rispetto a `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), quando devi impostare il valore Number o Cost.

**Returns:**
java.math.BigDecimal - il valore effettivo utilizzato per rappresentare il valore number o cost.
### getPhonetic() {#getPhonetic--}
```
public final String getPhonetic()
```


Restituisce le informazioni fonetiche sul nome del campo personalizzato.

**Returns:**
java.lang.String - le informazioni fonetiche sul nome del campo personalizzato.
### getStringValue() {#getStringValue--}
```
public final String getStringValue()
```


Restituisce il valore effettivo utilizzato per rappresentare una stringa di testo.

--------------------

Preferisci questa proprietà rispetto a `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), quando devi impostare il valore Text.

**Returns:**
java.lang.String - il valore effettivo utilizzato per rappresentare la stringa Text.
### getVal() {#getVal--}
```
public final String getVal()
```


Restituisce il valore effettivo nella rappresentazione interna. Preferisci utilizzare proprietà tipizzate fortemente elencate di seguito.

--------------------

Se vuoi impostare il valore Text, preferisci utilizzare la proprietà tipizzata fortemente `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)).

Se vuoi impostare il valore Number o Cost, preferisci utilizzare la proprietà tipizzata fortemente `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)).

Se vuoi impostare i valori Date/Start/Finish, preferisci utilizzare la proprietà tipizzata fortemente `DateValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)).

Se vuoi impostare il valore Duration, preferisci utilizzare la proprietà tipizzata fortemente `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)).

Se il tuo tipo non è elencato, utilizza la proprietà `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)).

**Returns:**
java.lang.String - il valore effettivo nella rappresentazione interna.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


Restituisce un GUID che identifica questo valore tra gli altri nell'intero progetto.

**Returns:**
java.util.UUID - un GUID che identifica questo valore tra gli altri in tutto il progetto.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Imposta il valore effettivo se può essere rappresentato come DateTime. Il valore predefinito è DateTime\#MinValue.MinValue.

--------------------

Preferisci questa proprietà rispetto a `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), quando devi impostare il valore DateTime.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | il valore effettivo se può essere rappresentato come DateTime. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


Imposta la descrizione di un valore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | la descrizione di un valore. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Imposta il valore effettivo utilizzato per rappresentare la Durata.

--------------------

Preferisci questa proprietà rispetto a `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), quando devi impostare il valore Duration.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | il valore effettivo utilizzato per rappresentare Duration. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Imposta l'identificatore univoco di un valore nell'intero progetto.

È importante non avere gli stessi identificatori per diverse istanze di [Value](../../com.aspose.tasks/value).

Il valore minimo di `Id`([getId()](../../com.aspose.tasks/value\#getId--)/[setId(int)](../../com.aspose.tasks/value\#setId-int-)) è `1`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | l'identificatore univoco di un valore in tutto il progetto. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Imposta il valore effettivo utilizzato per rappresentare un valore numerico o di costo.

--------------------

Preferisci questa proprietà rispetto a `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), quando devi impostare il valore Number o Cost.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | il valore effettivo utilizzato per rappresentare un numero o un valore di costo. |

### setPhonetic(String value) {#setPhonetic-java.lang.String-}
```
public final void setPhonetic(String value)
```


Imposta le informazioni fonetiche sul nome del campo personalizzato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | le informazioni fonetiche sul nome del campo personalizzato. |

### setStringValue(String value) {#setStringValue-java.lang.String-}
```
public final void setStringValue(String value)
```


Imposta il valore effettivo utilizzato per rappresentare una stringa di testo.

--------------------

Preferisci questa proprietà rispetto a `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)), quando devi impostare il valore Text.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | il valore effettivo utilizzato per rappresentare una stringa di testo. |

### setVal(String value) {#setVal-java.lang.String-}
```
public final void setVal(String value)
```


Imposta il valore effettivo nella rappresentazione interna. Preferisci utilizzare le proprietà tipizzate fortemente elencate di seguito.

--------------------

Se vuoi impostare il valore Text, preferisci utilizzare la proprietà tipizzata fortemente `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)).

Se vuoi impostare il valore Number o Cost, preferisci utilizzare la proprietà tipizzata fortemente `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)).

Se desideri impostare i valori Date/Start/Finish, preferisci utilizzare la proprietà tipizzata fortemente `DateTimeValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)).

Se vuoi impostare il valore Duration, preferisci utilizzare la proprietà tipizzata fortemente `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)).

Se il tuo tipo non è elencato, utilizza la proprietà `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | il valore effettivo nella rappresentazione interna. |

