---
title: "PrimaveraSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Consente di specificare opzioni aggiuntive durante il salvataggio del progetto nel formato Primavera XER."
type: docs
weight: 208
url: /it/java/com.aspose.tasks/primaverasaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraSaveOptions extends SimpleSaveOptions
```

Consente di specificare opzioni aggiuntive durante il salvataggio del progetto nel formato Primavera XER.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [PrimaveraSaveOptions()](#PrimaveraSaveOptions--) | Inizializza una nuova istanza della classe [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getActivityIdIncrement()](#getActivityIdIncrement--) | Ottiene l'incremento utilizzato nella rinumerazione degli ID delle attività. |
| [getActivityIdPrefix()](#getActivityIdPrefix--) | Ottiene il prefisso utilizzato nella rinumerazione degli ID delle attività. |
| [getActivityIdSuffix()](#getActivityIdSuffix--) | Ottiene il suffisso utilizzato nella rinumerazione degli ID delle attività. |
| [getRenumberActivityIds()](#getRenumberActivityIds--) | Ottiene un valore che indica se è necessario rinumerare gli ID delle attività. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Ottiene un valore che indica se le assegnazioni di risorse alle attività riepilogo devono essere ignorate durante l'esportazione. |
| [setActivityIdIncrement(int value)](#setActivityIdIncrement-int-) | Imposta l'incremento utilizzato nella rinumerazione degli ID delle attività. |
| [setActivityIdPrefix(String value)](#setActivityIdPrefix-java.lang.String-) | Imposta il prefisso utilizzato nella rinumerazione degli ID delle attività. |
| [setActivityIdSuffix(int value)](#setActivityIdSuffix-int-) | Imposta il suffisso utilizzato nella rinumerazione degli ID delle attività. |
| [setRenumberActivityIds(boolean value)](#setRenumberActivityIds-boolean-) | Imposta un valore che indica se è necessario rinumerare gli ID delle attività. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Imposta un valore che indica se le assegnazioni di risorse alle attività riepilogo devono essere ignorate durante l'esportazione. |
### PrimaveraSaveOptions() {#PrimaveraSaveOptions--}
```
public PrimaveraSaveOptions()
```


Inizializza una nuova istanza della classe [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions).

### getActivityIdIncrement() {#getActivityIdIncrement--}
```
public final int getActivityIdIncrement()
```


Ottiene l'incremento utilizzato nella rinumerazione degli ID delle attività.

**Returns:**
int - l'incremento utilizzato nella rinumerazione degli ID delle attività.
### getActivityIdPrefix() {#getActivityIdPrefix--}
```
public final String getActivityIdPrefix()
```


Ottiene il prefisso utilizzato nella rinumerazione degli ID delle attività.

**Returns:**
java.lang.String - il prefisso utilizzato nella rinumerazione degli ID delle attività.
### getActivityIdSuffix() {#getActivityIdSuffix--}
```
public final int getActivityIdSuffix()
```


Ottiene il suffisso utilizzato nella rinumerazione degli ID delle attività.

**Returns:**
int - il suffisso utilizzato nella rinumerazione degli ID delle attività.
### getRenumberActivityIds() {#getRenumberActivityIds--}
```
public final boolean getRenumberActivityIds()
```


Ottiene un valore che indica se è necessario rinumerare gli ID delle attività.

**Returns:**
boolean - un valore che indica se è necessario rinumerare gli ID delle attività.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Ottiene un valore che indica se le assegnazioni di risorse alle attività riepilogo devono essere ignorate durante l'esportazione.

Il software Primavera non supporta l'assegnazione di risorse alle attività di riepilogo (WBS). Pertanto, l'esportazione di tali assegnazioni può generare un file non valido secondo il modello di Primavera. Se true, le assegnazioni alle attività di riepilogo vengono omesse durante l'esportazione. Se false (il valore predefinito), viene generata un'eccezione se durante l'esportazione si incontra un'assegnazione a un'attività di riepilogo.

**Returns:**
boolean - un valore che indica se le assegnazioni di risorse alle attività di riepilogo devono essere omesse durante l'esportazione.
### setActivityIdIncrement(int value) {#setActivityIdIncrement-int-}
```
public final void setActivityIdIncrement(int value)
```


Imposta l'incremento utilizzato nella rinumerazione degli ID delle attività.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | l'incremento utilizzato nella rinumerazione degli ID delle attività. |

### setActivityIdPrefix(String value) {#setActivityIdPrefix-java.lang.String-}
```
public final void setActivityIdPrefix(String value)
```


Imposta il prefisso utilizzato nella rinumerazione degli ID delle attività.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | il prefisso utilizzato nella rinumerazione degli ID delle attività. |

### setActivityIdSuffix(int value) {#setActivityIdSuffix-int-}
```
public final void setActivityIdSuffix(int value)
```


Imposta il suffisso utilizzato nella rinumerazione degli ID delle attività.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il suffisso utilizzato nella rinumerazione degli ID delle attività. |

### setRenumberActivityIds(boolean value) {#setRenumberActivityIds-boolean-}
```
public final void setRenumberActivityIds(boolean value)
```


Imposta un valore che indica se è necessario rinumerare gli ID delle attività.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se è necessario rinumerare gli ID delle attività. |

### setSkipSummaryAssignments(boolean value) {#setSkipSummaryAssignments-boolean-}
```
public final void setSkipSummaryAssignments(boolean value)
```


Imposta un valore che indica se le assegnazioni di risorse alle attività riepilogo devono essere ignorate durante l'esportazione.

Il software Primavera non supporta l'assegnazione di risorse alle attività di riepilogo (WBS). Pertanto, l'esportazione di tali assegnazioni può generare un file non valido secondo il modello di Primavera. Se true, le assegnazioni alle attività di riepilogo vengono omesse durante l'esportazione. Se false (il valore predefinito), viene generata un'eccezione se durante l'esportazione si incontra un'assegnazione a un'attività di riepilogo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se le assegnazioni di risorse alle attività di riepilogo devono essere omesse durante l'esportazione. |

