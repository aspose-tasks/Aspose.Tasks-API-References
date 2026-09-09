---
title: "Tsk.Duration"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin girilen veya Microsoft Project tarafından başlangıç tarihi, bitiş tarihi, takvimler ve diğer zamanlama faktörlerine göre hesaplanan toplam aktif çalışma süresi."
type: docs
weight: 300
url: /tr/net/aspose.tasks/tsk/duration/
---
## Tsk.Duration field

Başlangıç tarihi, bitiş tarihi, takvimler ve diğer zamanlama faktörlerine göre Microsoft Project tarafından girilen veya hesaplanan bir görev için aktif çalışma süresinin toplam aralığı.

```csharp
public static readonly Key<Duration, TaskKey> Duration;
```

## Örnekler

Görevin süresini nasıl ayarlayacağınızı gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddTaskDuration_out.xml", SaveFileFormat.Xml);
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


