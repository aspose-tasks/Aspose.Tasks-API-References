---
title: "ResourceCollection sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ResourceCollection sınıfı. Resource nesnelerinin bir koleksiyonunu temsil eder"
type: docs
weight: 1770
url: /tr/net/aspose.tasks/resourcecollection/
---
## ResourceCollection class

[`Resource`](../resource/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class ResourceCollection : IList<Resource>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/resourcecollection/count/) { get; } | ResourceCollection içinde bulunan öğe sayısını alır. Salt okunur Int32. |
| [Item](../../aspose.tasks/resourcecollection/item/) { get; set; } | Belirtilen indeksteki öğeyi döndürür. |
| [ParentProject](../../aspose.tasks/resourcecollection/parentproject/) { get; } | ResourceCollection nesnesinin üst proje nesnesini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/resourcecollection/add/#add)() | Proje kaynakları koleksiyonunun son konumuna yeni bir kaynak ekler. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_1)(string) | Proje kaynakları koleksiyonunun son konumuna yeni bir kaynak ekler. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_2)(string, int) | Proje kaynakları koleksiyonunun belirtilen konumuna yeni bir kaynak ekler. |
| [Clear](../../aspose.tasks/resourcecollection/clear/)() | Doğrudan temizleme desteklenmez, bu yöntem sadece NotSupportedException fırlatır. |
| [GetById](../../aspose.tasks/resourcecollection/getbyid/)(int) | Belirtilen kimliğe (id) sahip bir kaynağı döndürür. |
| [GetByUid](../../aspose.tasks/resourcecollection/getbyuid/)(int) | Belirtilen Uid'ye sahip bir kaynağı döndürür. |
| [GetEnumerator](../../aspose.tasks/resourcecollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [Remove](../../aspose.tasks/resourcecollection/remove/)(Resource) | Bu, ICollection'ın Remove metodunun taslak (stub) uygulamasıdır ve yalnızca NotSupportedException fırlatır. |
| [ToList](../../aspose.tasks/resourcecollection/tolist/)() | ResourceCollection nesnesini [`Resource`](../resource/) nesnelerinin bir listesine dönüştürür. |

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

* class [Resource](../resource/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


