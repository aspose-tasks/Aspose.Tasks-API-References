---
title: "ITextStyleModificationCallback"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un callback che viene chiamato prima che TextStyle venga applicato a una cella di tabella."
type: docs
weight: 383
url: /it/java/com.aspose.tasks/itextstylemodificationcallback/
---
```
public interface ITextStyleModificationCallback
```

Rappresenta un callback che viene chiamato prima che TextStyle venga applicato a una cella di tabella.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)](#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-) | Il metodo da chiamare prima del rendering di una cella di tabella per una riga di attività nelle seguenti visualizzazioni: 'Gantt Chart', 'Task Sheet', 'Task Usage'. |
### beforeTaskTextStyleApplied(TaskTextStyleEventArgs args) {#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-}
```
public abstract void beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```


Il metodo da chiamare prima del rendering di una cella di tabella per una riga di attività nelle seguenti visualizzazioni: 'Gantt Chart', 'Task Sheet', 'Task Usage'.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| args | [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) | L'oggetto [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs). |

