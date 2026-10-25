---
title: "SplitPart.GetHashCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SplitPart yöntemi. SplitPart sınıfının örneği için bir karma kod değeri döndürür."
type: docs
weight: 40
url: /tr/net/aspose.tasks/splitpart/gethashcode/
---
## SplitPart.GetHashCode method

[`SplitPart`](../) sınıfının örneği için bir karma kod değeri döndürür.

```csharp
public override int GetHashCode()
```

### Dönüş Değeri

bu nesne için bir karma kod değeri döndürür.

## Örnekler

Bir bölünmüş parçanın karma kodunu nasıl alacağınızı gösterir.

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

// Bölünmüş parçaların eşitliği, parçaların başlangıç, bitiş ve indeksine karşı kontrol edilir.
var part1 = task.SplitParts[0];
var part2 = task.SplitParts[1];

// Bir bölünmüş parçanın başlangıç, bitiş ve indeksine dayalı karma kodu.
Console.WriteLine("Split Part 1 Start {0} Finish {1} HashCode {2}", part1.Start, part1.Finish, part1.GetHashCode());
Console.WriteLine("Split Part 2 Start {0} Finish {1} HashCode {2}", part2.Start, part2.Finish, part2.GetHashCode());
```

### Ayrıca Bakınız

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


