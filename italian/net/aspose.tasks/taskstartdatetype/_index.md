---
title: "Enum TaskStartDateType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.TaskStartDateType enum. Specifica il tipo della data di inizio di un'attività."
type: docs
weight: 2450
url: /it/net/aspose.tasks/taskstartdatetype/
---
## TaskStartDateType enumeration

Specifica il tipo della data di inizio di un'attività.

```csharp
public enum TaskStartDateType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Undefined | `-1` | Il valore del campo non era definito nel file di progetto originale. |
| ProjectStartDate | `0` | Data di inizio del progetto |
| CurrentDate | `1` | Data corrente |

## Osservazioni

Durante l'esportazione in XML i valori Undefined verranno eliminati dall'XML risultante.

## Esempi

Mostra come impostare la data di inizio predefinita dell'attività come 'CurrentDate'.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


