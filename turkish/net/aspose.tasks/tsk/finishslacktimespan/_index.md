---
title: "Tsk.FinishSlackTimeSpan"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Erken Bitiş ve Geç Bitiş tarihleri arasındaki süre"
type: docs
weight: 400
url: /tr/net/aspose.tasks/tsk/finishslacktimespan/
---
## Tsk.FinishSlackTimeSpan field

Erken Bitiş ve Geç Bitiş tarihleri arasındaki süre.

```csharp
public static readonly Key<TimeSpan, TaskKey> FinishSlackTimeSpan;
```

## Örnekler

Tsk.FinishSlackTimeSpan özelliğini nasıl okuyacağınızı gösterir. Özellik hesaplanır, bu yüzden genellikle açıkça ayarlamanıza gerek yoktur.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Finish Slack: " + task.Get(Tsk.FinishSlackTimeSpan));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


