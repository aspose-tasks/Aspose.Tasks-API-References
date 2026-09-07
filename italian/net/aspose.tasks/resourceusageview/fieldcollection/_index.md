---
title: "ResourceUsageView.FieldCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ResourceUsageView. Ottiene l'oggetto ResourceUsageViewFieldCollection di questo ResourceUsageView"
type: docs
weight: 10
url: /it/net/aspose.tasks/resourceusageview/fieldcollection/
---
## ResourceUsageView.FieldCollection property

Ottiene l'oggetto [`ResourceUsageViewFieldCollection`](../../resourceusageviewfieldcollection/) di questo ResourceUsageView.

```csharp
public ResourceUsageViewFieldCollection FieldCollection { get; }
```

## Esempi

Mostra come leggere i campi di visualizzazione dell'utilizzo delle risorse.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### Vedi anche

* class [ResourceUsageViewFieldCollection](../../resourceusageviewfieldcollection/)
* class [ResourceUsageView](../)
* namespace [Aspose.Tasks](../../resourceusageview/)
* assembly [Aspose.Tasks](../../../)


