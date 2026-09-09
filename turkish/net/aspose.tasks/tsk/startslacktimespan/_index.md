---
title: "Tsk.StartSlackTimeSpan"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Erken Başlangıç ve Geç Başlangıç tarihleri arasındaki süre"
type: docs
weight: 1020
url: /tr/net/aspose.tasks/tsk/startslacktimespan/
---
## Tsk.StartSlackTimeSpan field

Erken Başlangıç ve Geç Başlangıç tarihleri arasındaki süre.

```csharp
public static readonly Key<TimeSpan, TaskKey> StartSlackTimeSpan;
```

## Örnekler

Tsk.StartSlackTimeSpan özelliğini okuma nasıl yapılır gösterir. Özellik hesaplanır, bu yüzden genellikle açıkça ayarlamaya gerek yoktur.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Start Slack: " + task.Get(Tsk.StartSlackTimeSpan));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


