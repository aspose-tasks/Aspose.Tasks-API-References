---
title: "Task.SelectAllChildTasks"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task yöntemi. Bu görevin tüm alt görevlerini özyinelemeli olarak toplar"
type: docs
weight: 1400
url: /tr/net/aspose.tasks/task/selectallchildtasks/
---
## Task.SelectAllChildTasks method

Bu görevin tüm alt görevlerini özyinelemeli olarak toplar.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### Dönüş Değeri

Bu görevin alt görevlerinin bir listesi.

## Örnekler

Alt görevler üzerinde yineleme yapmayı gösterir.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

foreach (var tsk in project.RootTask.SelectAllChildTasks())
{
    Console.WriteLine("{0} {1}", tsk.Get(Tsk.Id), tsk.Get(Tsk.Name));
}
```

### Ayrıca Bakınız

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


