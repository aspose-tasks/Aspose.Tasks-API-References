---
title: "ResourceCollection.Add"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ResourceCollection. Добавляет новый ресурс в последнюю позицию коллекции ресурсов проекта."
type: docs
weight: 40
url: /ru/net/aspose.tasks/resourcecollection/add/
---
## Add() {#add}

Добавляет новый ресурс в последнюю позицию коллекции ресурсов проекта.

```csharp
public Resource Add()
```

### Возвращаемое значение

Ресурс добавлен.

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

---

## Add(string) {#add_1}

Добавляет новый ресурс в последнюю позицию коллекции ресурсов проекта.

```csharp
public Resource Add(string resourceName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| resourceName | Строка | Имя ресурса. |

### Возвращаемое значение

Ресурс добавлен.

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

---

## Add(string, int) {#add_2}

Добавляет новый ресурс в указанную позицию коллекции ресурсов проекта.

```csharp
public Resource Add(string resourceName, int beforeResourceId)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| resourceName | Строка | Имя ресурса. |
| beforeResourceId | Int32 | Позиция предыдущего ресурса в коллекции ресурсов проекта. |

### Возвращаемое значение

Ресурс добавлен.

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


