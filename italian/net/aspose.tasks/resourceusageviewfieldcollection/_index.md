---
title: "Classe ResourceUsageViewFieldCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.ResourceUsageViewFieldCollection. Rappresenta una collezione di valori ResourceUsageViewField"
type: docs
weight: 1830
url: /it/net/aspose.tasks/resourceusageviewfieldcollection/
---
## ResourceUsageViewFieldCollection class

Rappresenta una collezione di valori [`ResourceUsageViewField`](../resourceusageviewfield/).

```csharp
public class ResourceUsageViewFieldCollection : IList<ResourceUsageViewField>
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/resourceusageviewfieldcollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [ToList](../../aspose.tasks/resourceusageviewfieldcollection/tolist/)() | Converte l'istanza della classe `ResourceUsageViewFieldCollection` in un elenco contenente le istanze della classe [`ResourceUsageViewField`](../resourceusageviewfield/). |

## Esempi

Mostra come lavorare con la collezione di campi di un'istanza ResourceUsageView.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// si può trasformare la collezione in un elenco di ResourceUsageViewField
IList<ResourceUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### Vedi anche

* enum [ResourceUsageViewField](../resourceusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


