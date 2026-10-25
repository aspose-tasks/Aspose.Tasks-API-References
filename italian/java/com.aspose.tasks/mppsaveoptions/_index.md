---
title: "MPPSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Consente di specificare opzioni aggiuntive quando si salvano i dati del progetto in MPP."
type: docs
weight: 149
url: /it/java/com.aspose.tasks/mppsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class MPPSaveOptions extends SimpleSaveOptions
```

Consente di specificare opzioni aggiuntive quando si salvano i dati del progetto in MPP.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [MPPSaveOptions()](#MPPSaveOptions--) | Inizializza una nuova istanza della classe [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getClearVba()](#getClearVba--) | Restituisce un valore che indica se rimuovere i dati delle macro VBA esistenti durante il salvataggio di un progetto in formato MPP. |
| [getProtectionPassword()](#getProtectionPassword--) | Restituisce una password utilizzata per proteggere il file MPP risultante. |
| [getRemoveInvalidAssignments()](#getRemoveInvalidAssignments--) | Restituisce un valore che indica se rimuovere le assegnazioni di risorse non valide durante il salvataggio in MPP. |
| [getWriteFilters()](#getWriteFilters--) | Restituisce un valore che indica se scrivere i dati del filtro durante il salvataggio di un progetto in MPP per il formato. |
| [getWriteGroups()](#getWriteGroups--) | Ottiene un valore che indica se scrivere i dati dei gruppi durante il salvataggio di un progetto in formato MPP. |
| [getWriteVba()](#getWriteVba--) | Ottiene un valore che indica se aggiornare i dati delle macro VBA esistenti nel file MPP. |
| [getWriteViewData()](#getWriteViewData--) | Ottiene un valore che indica se scrivere i dati della vista durante il salvataggio di un progetto in formato MPP. |
| [setClearVba(boolean value)](#setClearVba-boolean-) | Imposta un valore che indica se rimuovere i dati delle macro VBA esistenti durante il salvataggio di un progetto in formato MPP. |
| [setProtectionPassword(String value)](#setProtectionPassword-java.lang.String-) | Imposta una password utilizzata per proteggere il file MPP risultante. |
| [setRemoveInvalidAssignments(boolean value)](#setRemoveInvalidAssignments-boolean-) | Imposta un valore che indica se rimuovere le assegnazioni di risorse non valide durante il salvataggio in MPP. |
| [setWriteFilters(boolean value)](#setWriteFilters-boolean-) | Imposta un valore che indica se scrivere i dati dei filtri durante il salvataggio di un progetto in formato MPP. |
| [setWriteGroups(boolean value)](#setWriteGroups-boolean-) | Imposta un valore che indica se scrivere i dati dei gruppi durante il salvataggio di un progetto in formato MPP. |
| [setWriteVba(boolean value)](#setWriteVba-boolean-) | Imposta un valore che indica se aggiornare i dati delle macro VBA esistenti nel file MPP. |
| [setWriteViewData(boolean value)](#setWriteViewData-boolean-) | Imposta un valore che indica se scrivere i dati della vista durante il salvataggio di un progetto in formato MPP. |
### MPPSaveOptions() {#MPPSaveOptions--}
```
public MPPSaveOptions()
```


Inizializza una nuova istanza della classe [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions).

### getClearVba() {#getClearVba--}
```
public final boolean getClearVba()
```


Restituisce un valore che indica se rimuovere i dati delle macro VBA esistenti durante il salvataggio di un progetto in formato MPP.

**Returns:**
boolean - un valore che indica se rimuovere i dati delle macro VBA esistenti durante il salvataggio di un progetto in formato MPP.
### getProtectionPassword() {#getProtectionPassword--}
```
public final String getProtectionPassword()
```


Ottiene una password utilizzata per proteggere il file MPP risultante. Attualmente è supportata per MS Project 2010 e formati più recenti.

--------------------

Il valore null indica che il file del progetto non è protetto.

**Returns:**
java.lang.String - una password utilizzata per proteggere il file MPP risultante.
### getRemoveInvalidAssignments() {#getRemoveInvalidAssignments--}
```
public final boolean getRemoveInvalidAssignments()
```


Restituisce un valore che indica se rimuovere le assegnazioni di risorse non valide durante il salvataggio in MPP.

--------------------

MS Project crea un'assegnazione di risorsa vuota per ogni attività. Imposta questo flag su true per rimuoverle al salvataggio.

**Returns:**
boolean - un valore che indica se rimuovere le assegnazioni di risorse non valide durante il salvataggio in MPP.
### getWriteFilters() {#getWriteFilters--}
```
public final boolean getWriteFilters()
```


Restituisce un valore che indica se scrivere i dati del filtro durante il salvataggio di un progetto in MPP per il formato.

--------------------

I dati dei filtri includono le collezioni Project.TaskFilters e Project.ResourceFilters.

--------------------

Attualmente supportato per MSP 2010 o formati più recenti.

**Returns:**
boolean - un valore che indica se scrivere i dati dei filtri durante il salvataggio di un progetto in formato MPP.
### getWriteGroups() {#getWriteGroups--}
```
public final boolean getWriteGroups()
```


Ottiene un valore che indica se scrivere i dati dei gruppi durante il salvataggio di un progetto in formato MPP.

--------------------

I dati dei gruppi includono le collezioni Project.TaskGroups e Project.ResourceGroups.

**Returns:**
boolean - un valore che indica se scrivere i dati dei gruppi durante il salvataggio di un progetto in formato MPP.
### getWriteVba() {#getWriteVba--}
```
public final boolean getWriteVba()
```


Ottiene un valore che indica se aggiornare i dati delle macro VBA esistenti nel file MPP. Attualmente è supportata la scrittura di VbaModule.SourceCode.

**Returns:**
boolean - un valore che indica se aggiornare i dati delle macro VBA esistenti nel file MPP.
### getWriteViewData() {#getWriteViewData--}
```
public final boolean getWriteViewData()
```


Ottiene un valore che indica se scrivere i dati della vista durante il salvataggio di un progetto in formato MPP.

--------------------

I dati della vista includono le collezioni Project.Views, Filters e Tables.

**Returns:**
boolean - un valore che indica se scrivere i dati della vista durante il salvataggio di un progetto in formato MPP.
### setClearVba(boolean value) {#setClearVba-boolean-}
```
public final void setClearVba(boolean value)
```


Imposta un valore che indica se rimuovere i dati delle macro VBA esistenti durante il salvataggio di un progetto in formato MPP.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se rimuovere i dati delle macro VBA esistenti durante il salvataggio di un progetto in formato MPP. |

### setProtectionPassword(String value) {#setProtectionPassword-java.lang.String-}
```
public final void setProtectionPassword(String value)
```


Imposta una password utilizzata per proteggere un file MPP risultante. Attualmente è supportata per MS Project 2010 e formati più recenti.

--------------------

Il valore null indica che il file del progetto non è protetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | una password utilizzata per proteggere un file MPP risultante. |

### setRemoveInvalidAssignments(boolean value) {#setRemoveInvalidAssignments-boolean-}
```
public final void setRemoveInvalidAssignments(boolean value)
```


Imposta un valore che indica se rimuovere le assegnazioni di risorse non valide durante il salvataggio in MPP.

--------------------

MS Project crea un'assegnazione di risorsa vuota per ogni attività. Imposta questo flag su true per rimuoverle al salvataggio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se rimuovere assegnazioni di risorse non valide durante il salvataggio in MPP. |

### setWriteFilters(boolean value) {#setWriteFilters-boolean-}
```
public final void setWriteFilters(boolean value)
```


Imposta un valore che indica se scrivere i dati dei filtri durante il salvataggio di un progetto in formato MPP.

--------------------

I dati dei filtri includono le collezioni Project.TaskFilters e Project.ResourceFilters.

--------------------

Attualmente supportato per MSP 2010 o formati più recenti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se scrivere i dati dei filtri durante il salvataggio di un progetto in formato MPP. |

### setWriteGroups(boolean value) {#setWriteGroups-boolean-}
```
public final void setWriteGroups(boolean value)
```


Imposta un valore che indica se scrivere i dati dei gruppi durante il salvataggio di un progetto in formato MPP.

--------------------

I dati dei gruppi includono le collezioni Project.TaskGroups e Project.ResourceGroups.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se scrivere i dati dei gruppi durante il salvataggio di un progetto in formato MPP. |

### setWriteVba(boolean value) {#setWriteVba-boolean-}
```
public final void setWriteVba(boolean value)
```


Imposta un valore che indica se aggiornare i dati delle macro VBA esistenti in un file MPP. Attualmente è supportata la scrittura di VbaModule.SourceCode.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se aggiornare i dati delle macro VBA esistenti in un file MPP. |

### setWriteViewData(boolean value) {#setWriteViewData-boolean-}
```
public final void setWriteViewData(boolean value)
```


Imposta un valore che indica se scrivere i dati della vista durante il salvataggio di un progetto in formato MPP.

--------------------

I dati della vista includono le collezioni Project.Views, Filters e Tables.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se scrivere i dati della vista durante il salvataggio di un progetto in formato MPP. |

