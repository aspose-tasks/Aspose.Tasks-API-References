---
title: "PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks for Java API Reference"
description: "Consente di specificare opzioni aggiuntive durante il salvataggio del progetto nel formato Primavera xml."
type: docs
weight: 212
url: /it/java/com.aspose.tasks/primaveraxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraXmlSaveOptions extends SimpleSaveOptions
```

Consente di specificare opzioni aggiuntive durante il salvataggio del progetto nel formato Primavera xml.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [PrimaveraXmlSaveOptions()](#PrimaveraXmlSaveOptions--) | Inizializza una nuova istanza della classe [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getSaveRootTask()](#getSaveRootTask--) | Ottiene un valore che indica se salvare o meno un'attività radice. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Ottiene un valore che indica se le assegnazioni di risorse alle attività riepilogo devono essere ignorate durante l'esportazione. |
| [setSaveRootTask(boolean value)](#setSaveRootTask-boolean-) | Imposta un valore che indica se salvare o meno un'attività radice. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Imposta un valore che indica se le assegnazioni di risorse alle attività riepilogo devono essere ignorate durante l'esportazione. |
### PrimaveraXmlSaveOptions() {#PrimaveraXmlSaveOptions--}
```
public PrimaveraXmlSaveOptions()
```


Inizializza una nuova istanza della classe [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions).

### getSaveRootTask() {#getSaveRootTask--}
```
public final boolean getSaveRootTask()
```


Ottiene un valore che indica se salvare o meno un'attività radice.

**Returns:**
boolean - un valore che indica se salvare o meno un'attività radice.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Ottiene un valore che indica se le assegnazioni di risorse alle attività riepilogo devono essere ignorate durante l'esportazione.

Il software Primavera non supporta l'assegnazione di risorse alle attività di riepilogo (WBS). Pertanto, l'esportazione di tali assegnazioni può generare un file non valido secondo il modello di Primavera. Se true, le assegnazioni alle attività di riepilogo vengono omesse durante l'esportazione. Se false (il valore predefinito), viene generata un'eccezione se durante l'esportazione si incontra un'assegnazione a un'attività di riepilogo.

**Returns:**
boolean - un valore che indica se le assegnazioni di risorse alle attività di riepilogo devono essere omesse durante l'esportazione.
### setSaveRootTask(boolean value) {#setSaveRootTask-boolean-}
```
public final void setSaveRootTask(boolean value)
```


Imposta un valore che indica se salvare o meno un'attività radice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se salvare o meno un'attività radice. |

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

