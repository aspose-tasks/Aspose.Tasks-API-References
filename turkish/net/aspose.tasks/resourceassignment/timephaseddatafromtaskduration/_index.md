---
title: "ResourceAssignment.TimephasedDataFromTaskDuration"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceAssignment yöntemi. Görev süresi ve planlanan başlangıç tarihine göre zaman aşamalı veri listesi oluşturur"
type: docs
weight: 780
url: /tr/net/aspose.tasks/resourceassignment/timephaseddatafromtaskduration/
---
## ResourceAssignment.TimephasedDataFromTaskDuration method

Görev süresi ve planlanan başlangıç tarihine dayanarak zaman aşamalı veri listesini oluşturur.

```csharp
public void TimephasedDataFromTaskDuration(Calendar calendar)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| takvim | Takvim | Zaman aşamalı verilerin oluşturulacağı takvim. |

## Örnekler

Bir görev için bölme eklemenin nasıl yapılacağını gösterir.

```csharp
var project = new Project();

// Standart bir takvim alın
var calendar = project.Get(Prj.Calendar);

// Projenin takvim ayarlarını belirleyin
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 4, 21, 17, 0, 0));

// Kök göreve yeni bir görev ekleyin
var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Duration, project.GetDuration(3));

// Yeni bir kaynak ataması oluşturun ve zaman aşamalı veri üretin
var assignment = project.ResourceAssignments.Add(task, null);
assignment.TimephasedDataFromTaskDuration(calendar);

// Görevi 3 parçaya bölün.
// Bölme için kullanılacak SplitTask yöntemine başlangıç ve bitiş tarihi argümanlarını sağlayın
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 16, 17, 0, 0), calendar);
assignment.SplitTask(new DateTime(2000, 3, 18, 8, 0, 0), new DateTime(2000, 3, 18, 17, 0, 0), calendar);
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

project.Save(OutDir + "CreateSplitTasks_out.xml", SaveFileFormat.Xml);
```

### Ayrıca Bakınız

* class [Calendar](../../calendar/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


