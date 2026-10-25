---
title: "ResourceAssignment.MakeTPs"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceAssignment yöntemi. Zaman aşamalı verilerin bir listesini oluşturur"
type: docs
weight: 740
url: /tr/net/aspose.tasks/resourceassignment/maketps/
---
## ResourceAssignment.MakeTPs method

Zaman aşamalı verilerin bir listesini oluşturur.

```csharp
public DateTime MakeTPs(DateTime start, TimeSpan time, Calendar calendar, 
    List<TimephasedData> list, bool isWorking, int type)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlangıç | DateTime | Belirtilen başlangıç tarihi. |
| zaman | TimeSpan | Belirtilen çalışma zamanı. |
| takvim | Takvim | Belirtilen çalışma takvimi. |
| liste | List`1 | Zaman aşamalı verilerin listesi. |
| isWorking | Boolean | Zaman aşamalı verilerin çalışıp çalışmadığını belirten belirtilen bayrak. |
| tür | Int32 | Belirtilen zaman aşamalı veri türü. |

### Dönüş Değeri

Liste boşsa listedeki maksimum tarih veya başlangıç tarihi.

## Örnekler

Parametrelerle TP'lerin nasıl oluşturulacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 3, 30, 8, 0, 0));
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2020, 4, 1, 8, 0, 0));

var tps = new List<TimephasedData>();
var lastDate = assignment.MakeTPs(
    assignment.Get(Asn.Start),
    TimeSpan.FromHours(32),
    project.Calendars.GetByName("Standard"),
    tps,
    true,
    (int)TimephasedDataType.AssignmentRemainingWork);

foreach (var data in tps)
{
    Console.WriteLine("Start: " + data.Start);
    Console.WriteLine("Finish: " + data.Finish);
    Console.WriteLine("TimephasedDataType: " + data.TimephasedDataType);
    Console.WriteLine();
}
```

### Ayrıca Bakınız

* class [Calendar](../../calendar/)
* class [TimephasedData](../../timephaseddata/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


