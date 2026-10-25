---
title: "Duration.TimeSpan"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Duration özelliği. Bu Duration nesnesinin TimeSpan örneğini alır. Bu Duration nesnesinin TimeSpan örneği."
type: docs
weight: 40
url: /tr/net/aspose.tasks/duration/timespan/
---
## Duration.TimeSpan property

`TimeSpan` örneğini bu Duration nesnesinden alır. Bu Duration nesnesinin TimeSpan örneği.

```csharp
public TimeSpan TimeSpan { get; }
```

## Örnekler

Bir süreyi zaman aralığına nasıl dönüştüreceğinizi gösterir.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// görev süresini al
var duration = task.Get(Tsk.Duration);
Console.WriteLine("Time span of duration: " + duration.TimeSpan);
```

### Ayrıca Bakınız

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


