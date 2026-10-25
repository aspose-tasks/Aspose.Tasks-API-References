---
title: "CustomProjectPropertyCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una raccolta di proprietà personalizzate del progetto."
type: docs
weight: 61
url: /it/java/com.aspose.tasks/customprojectpropertycollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection, com.aspose.tasks.PropertyKeyedCollection
```
public final class CustomProjectPropertyCollection extends PropertyKeyedCollection<CustomProjectProperty>
```

Rappresenta una raccolta di proprietà personalizzate del progetto.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [CustomProjectPropertyCollection()](#CustomProjectPropertyCollection--) | Inizializza una nuova istanza della classe [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | Crea una nuova proprietà personalizzata. |
| [add(String name, double value)](#add-java.lang.String-double-) | Crea una nuova proprietà personalizzata. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Crea una nuova proprietà personalizzata. |
| [add(String name, Date value)](#add-java.lang.String-java.util.Date-) | Crea una nuova proprietà personalizzata. |
| [clear()](#clear--) | Cancella la PropertyCollection. |
| [isReadOnly()](#isReadOnly--) | Ottiene un valore che indica se questa collezione è di sola lettura; altrimenti, false. |
| [remove(String name)](#remove-java.lang.String-) | Rimuove una proprietà con il nome specificato dalla collezione. |
### CustomProjectPropertyCollection() {#CustomProjectPropertyCollection--}
```
public CustomProjectPropertyCollection()
```


Inizializza una nuova istanza della classe [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection).

### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public final CustomProjectProperty add(String name, boolean value)
```


Crea una nuova proprietà personalizzata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà. |
| valore | boolean | Il valore dell'oggetto proprietà appena creato. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public final CustomProjectProperty add(String name, double value)
```


Crea una nuova proprietà personalizzata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà. |
| valore | double | Il valore dell'oggetto proprietà appena creato. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public final CustomProjectProperty add(String name, String value)
```


Crea una nuova proprietà personalizzata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà. |
| valore | java.lang.String | Il valore dell'oggetto proprietà appena creato. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, Date value) {#add-java.lang.String-java.util.Date-}
```
public final CustomProjectProperty add(String name, Date value)
```


Crea una nuova proprietà personalizzata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà. |
| valore | java.util.Date | Il valore dell'oggetto proprietà appena creato. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### clear() {#clear--}
```
public final void clear()
```


Cancella la PropertyCollection.

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Ottiene un valore che indica se questa collezione è di sola lettura; altrimenti, false.

**Returns:**
boolean - un valore che indica se questa collezione è di sola lettura; altrimenti, false.
### remove(String name) {#remove-java.lang.String-}
```
public final boolean remove(String name)
```


Rimuove una proprietà con il nome specificato dalla collezione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome della proprietà senza distinzione tra maiuscole e minuscole. |

**Returns:**
boolean - True se l'elemento è stato trovato e rimosso con successo; altrimenti, false.
