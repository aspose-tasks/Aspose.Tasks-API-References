---
title: "ResourceUsageViewFieldCollection.ToList"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ResourceUsageViewFieldCollection. Converte l'istanza della classe ResourceUsageViewFieldCollection in un elenco contenente le istanze della classe ResourceUsageViewField"
type: docs
weight: 20
url: /it/net/aspose.tasks/resourceusageviewfieldcollection/tolist/
---
## ResourceUsageViewFieldCollection.ToList method

Converte l'istanza della classe [`ResourceUsageViewFieldCollection`](../) in un elenco contenente le istanze della classe [`ResourceUsageViewField`](../../resourceusageviewfield/).

```csharp
public IList<ResourceUsageViewField> ToList()
```

### Valore di ritorno

L'istanza della classe [`ResourceUsageViewFieldCollection`](../) convertita in un elenco contenente le istanze della classe [`ResourceUsageViewField`](../../resourceusageviewfield/).

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

* enum [ResourceUsageViewField](../../resourceusageviewfield/)
* class [ResourceUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../resourceusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


