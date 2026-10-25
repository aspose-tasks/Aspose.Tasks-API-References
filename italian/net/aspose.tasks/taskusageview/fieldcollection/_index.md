---
title: "TaskUsageView.FieldCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà TaskUsageView. Ottiene l'oggetto TaskUsageViewFieldCollection di questo TaskUsageView"
type: docs
weight: 10
url: /it/net/aspose.tasks/taskusageview/fieldcollection/
---
## TaskUsageView.FieldCollection property

Ottiene l'oggetto [`TaskUsageViewFieldCollection`](../../taskusageviewfieldcollection/) di questo TaskUsageView.

```csharp
public TaskUsageViewFieldCollection FieldCollection { get; }
```

## Esempi

Mostra come leggere i campi della visualizzazione dell'uso delle attività.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### Vedi anche

* class [TaskUsageViewFieldCollection](../../taskusageviewfieldcollection/)
* class [TaskUsageView](../)
* namespace [Aspose.Tasks](../../taskusageview/)
* assembly [Aspose.Tasks](../../../)


