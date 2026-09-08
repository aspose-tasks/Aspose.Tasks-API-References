---
title: "Tsk.IsPublished"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет, должна ли текущая задача быть опубликована на Project Server вместе с остальной частью проекта"
type: docs
weight: 660
url: /ru/net/aspose.tasks/tsk/ispublished/
---
## Tsk.IsPublished field

Определяет, следует ли текущую задачу опубликовать на Project Server вместе с остальной частью проекта.

```csharp
public static readonly Key<NullableBool, TaskKey> IsPublished;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.IsPublished.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsPublished, true);

Console.WriteLine("Is Published: " + task.Get(Tsk.IsPublished));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


