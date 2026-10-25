---
title: "Task.Delete"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task yöntemi. Bir görevi üst proje görev koleksiyonundan ve tüm atamalarından siler"
type: docs
weight: 1320
url: /tr/net/aspose.tasks/task/delete/
---
## Task.Delete method

Görevi ana proje görev koleksiyonundan ve tüm atamalarından siler.

```csharp
public void Delete()
```

## Örnekler

Bir görevi nasıl sileceğinizi gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);

// bir görevi sil
task.Delete();

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);
```

### Ayrıca Bakınız

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


