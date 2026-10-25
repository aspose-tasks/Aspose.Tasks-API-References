---
title: "Task.OutlineOutdent"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task yöntemi. Görevi taslakta yükseltir"
type: docs
weight: 1390
url: /tr/net/aspose.tasks/task/outlineoutdent/
---
## Task.OutlineOutdent method

Taslakta bir görevi yükseltir.

```csharp
public void OutlineOutdent()
```

## Örnekler

Bir görevi dışa kaydırmanın nasıl yapılacağını gösterir.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = task1.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// görevi dışa kaydır
task2.OutlineOutdent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### Ayrıca Bakınız

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


