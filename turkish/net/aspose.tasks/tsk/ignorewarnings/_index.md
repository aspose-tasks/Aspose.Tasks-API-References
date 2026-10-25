---
title: "Tsk.IgnoreWarnings"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Microsoft Project'te zamanlama çakışması uyarı göstergesinin gizlenip gizlenmeyeceğini belirtir"
type: docs
weight: 540
url: /tr/net/aspose.tasks/tsk/ignorewarnings/
---
## Tsk.IgnoreWarnings field

Microsoft Project'te zamanlama çakışması uyarı göstergesinin gizlenip gizlenmeyeceğini gösterir.

```csharp
public static readonly Key<bool, TaskKey> IgnoreWarnings;
```

## Örnekler

Tsk.IgnoreWarnings özelliğini okuma/yazma nasıl yapılır gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreWarnings, true);

Console.WriteLine("Ignore Warnings: " + task.Get(Tsk.IgnoreWarnings));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


