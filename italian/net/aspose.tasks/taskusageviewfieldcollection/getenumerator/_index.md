---
title: "TaskUsageViewFieldCollection.GetEnumerator"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo TaskUsageViewFieldCollection. Restituisce un enumeratore per questa collezione"
type: docs
weight: 10
url: /it/net/aspose.tasks/taskusageviewfieldcollection/getenumerator/
---
## TaskUsageViewFieldCollection.GetEnumerator method

Restituisce un enumeratore per questa collezione.

```csharp
public IEnumerator<TaskUsageViewField> GetEnumerator()
```

### Valore di ritorno

un enumeratore per questa collezione.

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


