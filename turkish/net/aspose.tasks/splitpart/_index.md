---
title: "Sınıf SplitPart"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.SplitPart sınıfı. Bir görev bölümünü temsil eder. SplitPart, görevlerin SplitParts koleksiyonunun bir üyesidir."
type: docs
weight: 2290
url: /tr/net/aspose.tasks/splitpart/
---
## SplitPart class

Bir görev bölümünü temsil eder. SplitPart, görevin SplitParts koleksiyonunun bir üyesidir.

```csharp
public class SplitPart
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Finish](../../aspose.tasks/splitpart/finish/) { get; } | Bir SplitPart'ın bitiş tarihini alır. |
| [Start](../../aspose.tasks/splitpart/start/) { get; } | Bir SplitPart'ın başlangıç tarihini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../aspose.tasks/splitpart/equals/)(object) | İki bölünmüş parçayı karşılaştırır. |
| override [GetHashCode](../../aspose.tasks/splitpart/gethashcode/)() | `SplitPart` sınıfının örneği için bir hash kod değeri döndürür. |

## Örnekler

Bölünmüş bir görevin bölünmüş parçalarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 3, 21, 17, 0, 0));

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.IsManual, false);
task.Set(Tsk.Start, new DateTime(2000, 3, 15, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(3));

var assignment = project.ResourceAssignments.Add(task, project.Resources.Add("r1"));
assignment.Set(Asn.Start, new DateTime(2000, 3, 15, 8, 0, 0));
assignment.Set(Asn.Work, task.Get(Tsk.Work));
assignment.Set(Asn.Finish, new DateTime(2000, 3, 19, 17, 0, 0));

// önce kaynak atama zaman aşamalı verilerini oluşturmanız gerekir
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));

// görevi böl.
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// bölünmüş parçalar üzerinde yineleme yap
Console.WriteLine("Number of split parts: " + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("  Split Part Start: " + splitPart.Start);
    Console.WriteLine("  Split Part Finish: " + splitPart.Finish);
    Console.WriteLine();
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


