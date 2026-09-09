---
title: "Tsk.TotalSlackTimeSpan"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin bitiş tarihinin, projenin bitiş tarihini geciktirmeden gecikebileceği süre."
type: docs
weight: 1090
url: /tr/net/aspose.tasks/tsk/totalslacktimespan/
---
## Tsk.TotalSlackTimeSpan field

Görevin bitiş tarihinin, projenin bitiş tarihini geciktirmeden gecikebileceği süre.

```csharp
public static readonly Key<TimeSpan, TaskKey> TotalSlackTimeSpan;
```

## Örnekler

Tsk.TotalSlackTimeSpan özelliğini okuma nasıl yapılacağını gösterir. Özellik hesaplanır, bu yüzden genellikle açıkça ayarlamaya gerek yoktur.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Total Slack: " + task.Get(Tsk.TotalSlackTimeSpan));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


