---
title: "Tsk.FinishText"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Görevin bitiş metnini döndürür"
type: docs
weight: 410
url: /tr/net/aspose.tasks/tsk/finishtext/
---
## Tsk.FinishText field

Görevin bitiş metnini döndürür.

```csharp
public static readonly Key<string, TaskKey> FinishText;
```

## Örnekler

Tsk.FinishText özelliğini okuma/yazma yöntemini gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.FinishText, "Not A Finish");

Console.WriteLine("Finish Text: " + task.Get(Tsk.FinishText));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


