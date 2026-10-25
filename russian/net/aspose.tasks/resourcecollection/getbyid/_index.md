---
title: "ResourceCollection.GetById"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ResourceCollection. Возвращает ресурс с указанным id"
type: docs
weight: 60
url: /ru/net/aspose.tasks/resourcecollection/getbyid/
---
## ResourceCollection.GetById method

Возвращает ресурс с указанным идентификатором.

```csharp
public Resource GetById(int id)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| идентификатор | Int32 | Указанный id. |

### Возвращаемое значение

Ресурс с указанным id, если он присутствует; в противном случае null.

## Примечания

Сложность O(1).

## Примеры

Показывает, как работать с коллекциями ресурсов.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// добавить пустой ресурс
var resource = project.Resources.Add();
resource.Set(Rsc.Type, ResourceType.Work);

// добавить ресурс с именем
var developer = project.Resources.Add("Developer");
developer.Set(Rsc.Type, ResourceType.Work);

// добавить ресурс перед ресурсом с указанным ID
var manager = project.Resources.Add("Manager", developer.Get(Rsc.Id));
manager.Set(Rsc.Type, ResourceType.Work);

var devResource = project.Resources.GetById(4);
devResource.Set(Rsc.Code, "12345");

var manResource = project.Resources.GetByUid(4);
manResource.Set(Rsc.Code, "54321");

// получить ресурс по идентификатору
project.Resources.GetById(1);

Console.WriteLine("Print the resources of " + project.Resources.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Count of resources: " + project.Resources.Count);
foreach (var rsc in project.Resources)
{
    Console.WriteLine("Resource Name: " + rsc.Get(Rsc.Name));
}

Console.WriteLine();

// коллекции ресурсов не поддерживают операцию Clear
// project.Resources.Clear();
// используйте следующий пример кода вместо
List<Resource> list = project.Resources.ToList();
foreach (var rsc in list)
{
    rsc.Delete();
}
```

### См. также

* class [Resource](../../resource/)
* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)


