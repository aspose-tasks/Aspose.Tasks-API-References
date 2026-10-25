---
title: "Task.Predecessors"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task özelliği. Bu Task nesnesinin tüm öncüllerini içeren bir TaskCollection nesnesi alır"
type: docs
weight: 980
url: /tr/net/aspose.tasks/task/predecessors/
---
## Task.Predecessors property

Bu Task nesnesinin tüm öncüllerini içeren bir [`TaskCollection`](../../taskcollection/) nesnesi alır.

```csharp
public TaskCollection Predecessors { get; }
```

### Dönüş Değeri

Salt okunur bir [`TaskCollection`](../../taskcollection/) sınıf örneği.

## Örnekler

Görevin öncüllerinin nasıl okunacağını gösterir.

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var predecessor in succ.Predecessors)
{
    Console.WriteLine("{0} {1}", predecessor.Get(Tsk.Id), predecessor.Get(Tsk.Name));
}
```

### Ayrıca Bakınız

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


