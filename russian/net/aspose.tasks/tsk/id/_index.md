---
title: "Tsk.Id"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Идентификатор позиции задачи в списке задач"
type: docs
weight: 520
url: /ru/net/aspose.tasks/tsk/id/
---
## Tsk.Id field

Идентификатор позиции задачи в списке задач.

```csharp
public static readonly Key<int, TaskKey> Id;
```

## Примеры

Показывает, как читать/записывать свойства задачи.

```csharp
var project = new Project();

// Добавьте задачу и задайте свойства задачи
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Проанализировать все собранные задачи
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


