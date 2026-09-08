---
title: "Task.Get"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Task. Возвращает значение, к которому свойство сопоставлено в этом контейнере"
type: docs
weight: 1340
url: /ru/net/aspose.tasks/task/get/
---
## Task.Get&lt;T&gt; method

Возвращает значение, к которому свойство сопоставлено в этом контейнере.

```csharp
public T Get<T>(Key<T, TaskKey> key)
```

| Параметр | Описание |
| --- | --- |
| T | тип сопоставленного значения. |
| key | указанный ключ свойства. [`Tsk`](../../tsk/) для получения ключа свойства. |

### Возвращаемое значение

значение, к которому свойство сопоставлено в этом контейнере.

## Примеры

Показывает, как получать/устанавливать свойства задачи.

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
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


