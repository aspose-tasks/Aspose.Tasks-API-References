---
title: "ResourceAssignment.TimephasedData"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ResourceAssignment. Получает или задает экземпляр класса TimephasedDataCollection, содержащий элементы класса TimephasedData"
type: docs
weight: 600
url: /ru/net/aspose.tasks/resourceassignment/timephaseddata/
---
## ResourceAssignment.TimephasedData property

Получает или задает экземпляр класса [`TimephasedDataCollection`](../../timephaseddatacollection/), содержащий элементы класса `TimephasedData`.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Примеры

Показывает, как читать данные с разбивкой по времени назначения ресурса.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");
project.Set(Prj.StartDate, new DateTime(2013, 10, 30, 9, 0, 0));
project.Set(Prj.NewTasksAreManual, false);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Duration, project.GetDuration(6));

var rsc = project.Resources.Add("Rsc");
rsc.Set(Rsc.StandardRate, 10);
rsc.Set(Rsc.OvertimeRate, 15);

// Создать назначение ресурса
var assn = project.ResourceAssignments.Add(task, rsc);
assn.Set(Asn.Stop, DateTime.MinValue);
assn.Set(Asn.Resume, DateTime.MinValue);
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

// получить временные данные
foreach (var td in assn.TimephasedData)
{
    Console.WriteLine(td.Value);
}
```

### См. также

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


