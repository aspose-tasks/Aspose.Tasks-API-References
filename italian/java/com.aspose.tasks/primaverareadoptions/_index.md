---
title: "PrimaveraReadOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Consente di specificare opzioni aggiuntive durante la lettura dei file Primavera Xml o Primavera Xer."
type: docs
weight: 206
url: /it/java/com.aspose.tasks/primaverareadoptions/
---

**Inheritance:**
java.lang.Object
```
public class PrimaveraReadOptions
```

Consente di specificare opzioni aggiuntive durante la lettura dei file Primavera Xml o Primavera Xer.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [PrimaveraReadOptions()](#PrimaveraReadOptions--) | Inizializza una nuova istanza della classe [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getPreserveUids()](#getPreserveUids--) | Restituisce un flag che specifica se gli identificatori univoci originali delle entità devono essere conservati. |
| [getProjectUid()](#getProjectUid--) | Restituisce l'UID di un progetto da leggere da un file contenente più progetti. |
| [getReadBaselineProjects()](#getReadBaselineProjects--) | Restituisce un flag che specifica se i progetti di baseline devono essere caricati. |
| [getUndefinedConstraintHandlingBehavior()](#getUndefinedConstraintHandlingBehavior--) | Specifica il comportamento utilizzato per elaborare le attività con vincoli non definiti letti dal formato XER. |
| [setPreserveUids(boolean value)](#setPreserveUids-boolean-) | Imposta un flag che specifica se gli identificatori univoci originali delle entità devono essere conservati. |
| [setProjectUid(int value)](#setProjectUid-int-) | Imposta l'UID di un progetto da leggere da un file contenente più progetti. |
| [setReadBaselineProjects(boolean value)](#setReadBaselineProjects-boolean-) | Imposta un flag che specifica se i progetti di baseline devono essere caricati. |
| [setUndefinedConstraintHandlingBehavior(int value)](#setUndefinedConstraintHandlingBehavior-int-) | Specifica il comportamento utilizzato per elaborare le attività con vincoli non definiti letti dal formato XER. |
### PrimaveraReadOptions() {#PrimaveraReadOptions--}
```
public PrimaveraReadOptions()
```


Inizializza una nuova istanza della classe [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions).

### getPreserveUids() {#getPreserveUids--}
```
public final boolean getPreserveUids()
```


Restituisce un flag che specifica se gli identificatori univoci originali delle entità devono essere conservati.

**Returns:**
boolean - un flag che specifica se gli identificatori univoci originali delle entità devono essere conservati.
### getProjectUid() {#getProjectUid--}
```
public final int getProjectUid()
```


Restituisce l'UID di un progetto da leggere da un file contenente più progetti.

**Returns:**
int - l'UID di un progetto da leggere da un file contenente più progetti.
### getReadBaselineProjects() {#getReadBaselineProjects--}
```
public final boolean getReadBaselineProjects()
```


Restituisce un flag che specifica se i progetti di baseline devono essere caricati. Il valore predefinito è true.

--------------------

Il flag è applicabile ai file Primavera XML contenenti progetti di baseline (le baseline non sono supportate dal formato XER). L'opzione può essere impostata su false per velocizzare il caricamento di un progetto grande con baseline quando i dati di baseline non sono necessari.

**Returns:**
boolean - un flag che specifica se i progetti di baseline devono essere caricati.
### getUndefinedConstraintHandlingBehavior() {#getUndefinedConstraintHandlingBehavior--}
```
public final int getUndefinedConstraintHandlingBehavior()
```


Specifica il comportamento utilizzato per elaborare le attività con vincoli non definiti letti dal formato XER.

**Returns:**
int - il comportamento utilizzato per elaborare le attività con vincoli non definiti letti dal formato XER.
### setPreserveUids(boolean value) {#setPreserveUids-boolean-}
```
public final void setPreserveUids(boolean value)
```


Imposta un flag che specifica se gli identificatori univoci originali delle entità devono essere conservati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un flag che specifica se gli identificatori univoci originali delle entità devono essere conservati. |

### setProjectUid(int value) {#setProjectUid-int-}
```
public final void setProjectUid(int value)
```


Imposta l'UID di un progetto da leggere da un file contenente più progetti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | l'UID di un progetto da leggere da un file contenente più progetti. |

### setReadBaselineProjects(boolean value) {#setReadBaselineProjects-boolean-}
```
public final void setReadBaselineProjects(boolean value)
```


Imposta un flag che specifica se i progetti baseline devono essere caricati. Il valore predefinito è true.

--------------------

Il flag è applicabile ai file Primavera XML contenenti progetti di baseline (le baseline non sono supportate dal formato XER). L'opzione può essere impostata su false per velocizzare il caricamento di un progetto grande con baseline quando i dati di baseline non sono necessari.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un flag che specifica se i progetti baseline devono essere caricati. |

### setUndefinedConstraintHandlingBehavior(int value) {#setUndefinedConstraintHandlingBehavior-int-}
```
public final void setUndefinedConstraintHandlingBehavior(int value)
```


Specifica il comportamento utilizzato per elaborare le attività con vincoli non definiti letti dal formato XER.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il comportamento utilizzato per elaborare attività con vincoli non definiti letti dal formato XER. |

