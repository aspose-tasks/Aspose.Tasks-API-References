---
title: "Task.ParentProject"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Task. Получает родительский проект задачи"
type: docs
weight: 930
url: /ru/net/aspose.tasks/task/parentproject/
---
## Task.ParentProject property

Получает родительский проект задачи.

```csharp
public Project ParentProject { get; }
```

## Примечания

Вызовите Project.UpdateReferences, чтобы обновить эти свойства.

## Примеры

Показывает, как использовать родительский проект задачи.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Parent");

// Установите длительность задачи, используя тип единицы времени проекта по умолчанию.
task.Set(Tsk.Duration, task.ParentProject.GetDuration(1));

Console.WriteLine(task.Get(Tsk.Duration));
```

### См. также

* class [Project](../../project/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


