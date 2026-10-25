---
title: "Resource.ParentProject"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Resource. Получает родительский проект для этого контейнера"
type: docs
weight: 600
url: /ru/net/aspose.tasks/resource/parentproject/
---
## Resource.ParentProject property

Получает родительский проект для этого контейнера.

```csharp
public Project ParentProject { get; }
```

## Примеры

Показывает, как использовать родительский проект ресурса.

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

// Устанавливает работу для ресурса, используя тип единицы времени работы проекта по умолчанию.
resource.Set(Rsc.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resource.Get(Rsc.Work));
```

### См. также

* class [Project](../../project/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


