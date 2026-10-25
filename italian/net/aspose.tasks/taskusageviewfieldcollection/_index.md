---
title: "Classe TaskUsageViewFieldCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.TaskUsageViewFieldCollection. Rappresenta una raccolta di valori TaskUsageViewField"
type: docs
weight: 2500
url: /it/net/aspose.tasks/taskusageviewfieldcollection/
---
## TaskUsageViewFieldCollection class

Rappresenta una raccolta di valori [`TaskUsageViewField`](../taskusageviewfield/).

```csharp
public class TaskUsageViewFieldCollection : IList<TaskUsageViewField>
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/taskusageviewfieldcollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [ToList](../../aspose.tasks/taskusageviewfieldcollection/tolist/)() | Restituisce un elenco che contiene tutti gli elementi di questa raccolta. |

## Esempi

Mostra come lavorare con la raccolta di campi di un'istanza di TaskUsageView.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// È possibile trasformare la raccolta in un elenco di TaskUsageViewField
IList<TaskUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### Vedi anche

* enum [TaskUsageViewField](../taskusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


