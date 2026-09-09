---
title: "Task.Successors"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task özelliği. Bu Task nesnesinin tüm ardılılarını içeren bir TaskCollection nesnesi alır"
type: docs
weight: 1200
url: /tr/net/aspose.tasks/task/successors/
---
## Task.Successors property

Bu Task nesnesinin tüm ardılılarını içeren bir [`TaskCollection`](../../taskcollection/) nesnesi alır.

```csharp
public TaskCollection Successors { get; }
```

### Dönüş Değeri

Salt okunur bir [`TaskCollection`](../../taskcollection/) sınıf örneği.

## Örnekler

Görev ardıllarını nasıl okuyacağınızı gösterir.

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var successor in pred.Successors)
{
    Console.WriteLine("{0} {1}", successor.Get(Tsk.Id), successor.Get(Tsk.Name));
}
```

### Ayrıca Bakınız

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


