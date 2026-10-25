---
title: "Klasse TaskUsageViewFieldCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TaskUsageViewFieldCollection-klasse. Vertegenwoordigt een verzameling van TaskUsageViewField-waarden"
type: docs
weight: 2500
url: /nl/net/aspose.tasks/taskusageviewfieldcollection/
---
## TaskUsageViewFieldCollection class

Vertegenwoordigt een verzameling van [`TaskUsageViewField`](../taskusageviewfield/) waarden.

```csharp
public class TaskUsageViewFieldCollection : IList<TaskUsageViewField>
```

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/taskusageviewfieldcollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [ToList](../../aspose.tasks/taskusageviewfieldcollection/tolist/)() | Retourneert een lijst die alle items uit deze verzameling bevat. |

## Voorbeelden

Toont hoe te werken met de veldverzameling van een TaskUsageView‑instantie.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// men kan de verzameling omzetten in een lijst van TaskUsageViewField
IList<TaskUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### Zie ook

* enum [TaskUsageViewField](../taskusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


