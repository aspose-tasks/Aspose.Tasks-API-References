---
title: "Tsk.FreeSlackTimeSpan"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin, sonraki görevleri geciktirmeden gecikebileceği süre."
type: docs
weight: 450
url: /tr/net/aspose.tasks/tsk/freeslacktimespan/
---
## Tsk.FreeSlackTimeSpan field

Bir görevin, sonraki görevleri geciktirmeden gecikebileceği süre.

```csharp
public static readonly Key<TimeSpan, TaskKey> FreeSlackTimeSpan;
```

## Örnekler

Tsk.FreeSlackTimeSpan özelliğini okuma nasıl yapılacağını gösterir. Özellik hesaplanır, bu yüzden genellikle açıkça ayarlamaya gerek yoktur.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Free Slack: " + task.Get(Tsk.FreeSlackTimeSpan));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


