---
title: "Task.OutlineIndent"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task metodu. Görevi taslakta girintiler"
type: docs
weight: 1380
url: /tr/net/aspose.tasks/task/outlineindent/
---
## Task.OutlineIndent method

Taslakta bir görevi girintiler.

```csharp
public void OutlineIndent()
```

## Örnekler

Bir görevin nasıl girintileneceğini gösterir.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = project.RootTask.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// görevi girintile
task2.OutlineIndent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### Ayrıca Bakınız

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


