---
title: "Класс ResourceCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ResourceCollection. Представляет коллекцию объектов Resource"
type: docs
weight: 1770
url: /ru/net/aspose.tasks/resourcecollection/
---
## ResourceCollection class

Представляет коллекцию объектов [`Resource`](../resource/).

```csharp
public class ResourceCollection : IList<Resource>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/resourcecollection/count/) { get; } | Получает количество элементов, содержащихся в ResourceCollection. Только для чтения Int32. |
| [Item](../../aspose.tasks/resourcecollection/item/) { get; set; } | Возвращает элемент по указанному индексу. |
| [ParentProject](../../aspose.tasks/resourcecollection/parentproject/) { get; } | Получает родительский проект объекта ResourceCollection. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/resourcecollection/add/#add)() | Добавляет новый ресурс в последнюю позицию коллекции ресурсов проекта. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_1)(string) | Добавляет новый ресурс в последнюю позицию коллекции ресурсов проекта. |
| [Add](../../aspose.tasks/resourcecollection/add/#add_2)(string, int) | Добавляет новый ресурс в указанную позицию коллекции ресурсов проекта. |
| [Clear](../../aspose.tasks/resourcecollection/clear/)() | Прямое очищение не поддерживается, этот метод просто бросает NotSupportedException. |
| [GetById](../../aspose.tasks/resourcecollection/getbyid/)(int) | Возвращает ресурс с указанным идентификатором. |
| [GetByUid](../../aspose.tasks/resourcecollection/getbyuid/)(int) | Возвращает ресурс с указанным Uid. |
| [GetEnumerator](../../aspose.tasks/resourcecollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [Remove](../../aspose.tasks/resourcecollection/remove/)(Resource) | Это заглушка реализации метода Remove интерфейса ICollection, который только бросает NotSupportedException. |
| [ToList](../../aspose.tasks/resourcecollection/tolist/)() | Преобразует объект ResourceCollection в список объектов [`Resource`](../resource/). |

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

* class [Resource](../resource/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


