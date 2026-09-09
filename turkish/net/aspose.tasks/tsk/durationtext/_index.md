---
title: "Tsk.DurationText"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Görevin süre metnini döndürür"
type: docs
weight: 310
url: /tr/net/aspose.tasks/tsk/durationtext/
---
## Tsk.DurationText field

Görevin süre metnini döndürür.

```csharp
public static readonly Key<string, TaskKey> DurationText;
```

## Örnekler

Tsk.DurationText özelliğini okuma/yazma nasıl yapılır gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationText, "Not A Duration");

Console.WriteLine("Duration Text: " + task.Get(Tsk.DurationText));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


