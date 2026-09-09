---
title: "Tsk.ActualFinish"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin tamamlandığı tarih."
type: docs
weight: 40
url: /tr/net/aspose.tasks/tsk/actualfinish/
---
## Tsk.ActualFinish field

Görevin tamamlandığı tarih.

```csharp
public static readonly Key<DateTime, TaskKey> ActualFinish;
```

## Örnekler

Proje tarihlerinin değerlendirme modunda sıfırlandığını gösterir.

```csharp
var project = new Project();

// yeni görevler oluştur
var task1 = project.RootTask.Children.Add("Task1");
task1.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task1.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

var task2 = project.RootTask.Children.Add("Task2");
task2.Set(Tsk.ActualStart, new DateTime(2000, 2, 10, 8, 0, 0));
task2.Set(Tsk.ActualFinish, new DateTime(2000, 2, 10, 17, 0, 0));

project.Save(OutDir + "EvaluationDateTimeLimitations_out.xml", SaveFileFormat.Xml);
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


