---
title: "Tsk.ConstraintType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevi zamanlamada uygulanabilecek kısıtlama türü için seçenekler sağlar."
type: docs
weight: 210
url: /tr/net/aspose.tasks/tsk/constrainttype/
---
## Tsk.ConstraintType field

Bir görevi zamanlamada uygulanabilecek kısıtlama türü için seçenekler sunar.

```csharp
public static readonly Key<ConstraintType, TaskKey> ConstraintType;
```

## Örnekler

Bir görev için kısıtlama nasıl alınır/ayarlanır gösterir.

```csharp
var project = new Project(DataDir + "ConstraintAsLateAsPossible.mpp");

// Id 11 olan görev için kısıtlamayı Mümkün Olduğunca Geç Olarak ayarla
var newTask = project.RootTask.Children.GetById(11);
newTask.Set(Tsk.ConstraintType, ConstraintType.AsLateAsPossible);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Toplanan tüm görevleri ayrıştır
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.ConstraintType).ToString());
    Console.WriteLine(task.Get(Tsk.ConstraintDate).ToShortDateString() == "1/1/2000" ? "NA" : task.Get(Tsk.ConstraintDate).ToShortDateString());
}

SaveOptions options = new PdfSaveOptions
{
    StartDate = project.Get(Prj.StartDate),
    Timescale = Timescale.ThirdsOfMonths
};

project.Save(OutDir + "SetConstraintAsLateAsPossible_out.pdf", options);
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [ConstraintType](../../constrainttype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


