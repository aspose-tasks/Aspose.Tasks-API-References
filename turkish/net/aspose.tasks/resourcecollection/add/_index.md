---
title: "ResourceCollection.Add"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceCollection yöntemi. Proje kaynakları koleksiyonunun son konumuna yeni bir kaynak ekler"
type: docs
weight: 40
url: /tr/net/aspose.tasks/resourcecollection/add/
---
## Add() {#add}

Proje kaynakları koleksiyonunun son konumuna yeni bir kaynak ekler.

```csharp
public Resource Add()
```

### Dönüş Değeri

Kaynak eklendi.

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

* class [Resource](../../resource/)
* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string) {#add_1}

Proje kaynakları koleksiyonunun son konumuna yeni bir kaynak ekler.

```csharp
public Resource Add(string resourceName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| resourceName | Dize | Bir kaynağın adı. |

### Dönüş Değeri

Kaynak eklendi.

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

* class [Resource](../../resource/)
* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_2}

Proje kaynakları koleksiyonunun belirtilen konumuna yeni bir kaynak ekler.

```csharp
public Resource Add(string resourceName, int beforeResourceId)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| resourceName | Dize | Bir kaynağın adı. |
| beforeResourceId | Int32 | Bir proje kaynak koleksiyonundaki önceki kaynağın konumu. |

### Dönüş Değeri

Kaynak eklendi.

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

* class [Resource](../../resource/)
* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)


