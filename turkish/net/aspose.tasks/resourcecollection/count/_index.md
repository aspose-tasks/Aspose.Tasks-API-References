---
title: "ResourceCollection.Count"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceCollection özelliği. ResourceCollection içinde bulunan öğe sayısını alır. Salt okunur Int32"
type: docs
weight: 10
url: /tr/net/aspose.tasks/resourcecollection/count/
---
## ResourceCollection.Count property

ResourceCollection içinde bulunan öğe sayısını alır. Salt okunur Int32.

```csharp
public int Count { get; }
```

## Örnekler

Kaynak koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// boş kaynak ekle
var resource = project.Resources.Add();
resource.Set(Rsc.Type, ResourceType.Work);

// adlı kaynak ekle
var developer = project.Resources.Add("Developer");
developer.Set(Rsc.Type, ResourceType.Work);

// belirtilen ID'ye sahip kaynağın önüne kaynak ekle
var manager = project.Resources.Add("Manager", developer.Get(Rsc.Id));
manager.Set(Rsc.Type, ResourceType.Work);

var devResource = project.Resources.GetById(4);
devResource.Set(Rsc.Code, "12345");

var manResource = project.Resources.GetByUid(4);
manResource.Set(Rsc.Code, "54321");

// kaynağı id ile al
project.Resources.GetById(1);

Console.WriteLine("Print the resources of " + project.Resources.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Count of resources: " + project.Resources.Count);
foreach (var rsc in project.Resources)
{
    Console.WriteLine("Resource Name: " + rsc.Get(Rsc.Name));
}

Console.WriteLine();

// kaynak koleksiyonları Clear işlemini desteklemez
// project.Resources.Clear();
// bunun yerine sonraki kod örneğini kullanın
List<Resource> list = project.Resources.ToList();
foreach (var rsc in list)
{
    rsc.Delete();
}
```

### Ayrıca Bakınız

* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)


