---
title: "TaskUsageViewFieldCollection.ToList"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo TaskUsageViewFieldCollection. Restituisce un elenco che contiene tutti gli elementi di questa collezione"
type: docs
weight: 20
url: /it/net/aspose.tasks/taskusageviewfieldcollection/tolist/
---
## TaskUsageViewFieldCollection.ToList method

Restituisce un elenco che contiene tutti gli elementi di questa raccolta.

```csharp
public IList<TaskUsageViewField> ToList()
```

### Valore di ritorno

restituisce un elenco che contiene tutti gli elementi di questa collezione.

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

* enum [TaskUsageViewField](../../taskusageviewfield/)
* class [TaskUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../taskusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


