---
title: "Tsk.IsActive"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет, активна ли задача. Неактивные задачи больше не влияют на другие задачи или общий график проекта"
type: docs
weight: 550
url: /ru/net/aspose.tasks/tsk/isactive/
---
## Tsk.IsActive field

Определяет, является ли задача активной. Неактивные задачи больше не влияют на другие задачи или общий график проекта.

```csharp
public static readonly Key<NullableBool, TaskKey> IsActive;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.IsActive.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsActive, true);

Console.WriteLine("Is Active: " + task.Get(Tsk.IsActive));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


