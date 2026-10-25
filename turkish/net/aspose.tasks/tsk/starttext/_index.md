---
title: "Tsk.StartText"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Görevin başlangıç metnini döndürür."
type: docs
weight: 1030
url: /tr/net/aspose.tasks/tsk/starttext/
---
## Tsk.StartText field

Görevin başlangıç metnini döndürür.

```csharp
public static readonly Key<string, TaskKey> StartText;
```

## Örnekler

Tsk.StartText özelliğini okuma/yazma nasıl yapılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StartText, "Start Task Text");

Console.WriteLine("Start Text: " + task.Get(Tsk.StartText));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


