---
title: "ResourceAssignment.GetTimephasedData"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ResourceAssignment. Возвращает экземпляр класса TimephasedDataCollection, содержащий экземпляры класса TimephasedData в заданных начальной и конечной датах указанного TimephasedDataType"
type: docs
weight: 720
url: /ru/net/aspose.tasks/resourceassignment/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Возвращает экземпляр класса [`TimephasedDataCollection`](../../timephaseddatacollection/) , содержащий экземпляры класса [`TimephasedData`](../timephaseddata/) в заданных начальной и конечной датах указанного [`TimephasedDataType`](../../timephaseddatatype/).

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| start | DateTime | Дата начала для данных с фазированием во времени. |
| end | DateTime | Дата окончания для данных с фазированием во времени. |
| timephasedType | TimephasedDataType | Тип данных с фазированием во времени ([`TimephasedDataType`](../../timephaseddatatype/)). |

### Возвращаемое значение

возвращает список, содержащий экземпляры класса [`TimephasedData`](../../timephaseddata/).

## Примеры

Показывает, как сгенерировать временные данные назначения ресурса в пределах диапазона дат.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// Установить свойства проекта
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

// Установить контур Backloaded, он увеличивает длительность задачи с 6 до 10 дней
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// получить временные данные
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### См. также

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Возвращает объект [`TimephasedDataCollection`](../../timephaseddatacollection/) с экземплярами класса [`TimephasedData`](../timephaseddata/) в заданных начальной и конечной датах AssignmentWork.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| start | DateTime | Дата начала для данных с фазированием во времени. |
| end | DateTime | Дата окончания для данных с фазированием во времени. |

### Возвращаемое значение

возвращает список, содержащий экземпляры класса [`TimephasedData`](../../timephaseddata/).

## Примеры

Показывает, как сгенерировать временные данные назначения ресурса в пределах диапазона дат.

```csharp
var project = new Project(DataDir + "ReadWriteTimephasedData.mpp");

// Установить свойства проекта
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

// Установить контур Backloaded, он увеличивает длительность задачи с 6 до 10 дней
assn.Set(Asn.WorkContour, WorkContourType.BackLoaded);

project.SetBaseline(BaselineType.Baseline);
task.Set(Tsk.PercentComplete, 50);

// получить временные данные
List<TimephasedData> td = assn.GetTimephasedData(assn.Get(Asn.Start), assn.Get(Asn.Finish), TimephasedDataType.AssignmentRemainingWork).ToList();
Console.WriteLine(td.Count);
foreach (var timePhasedValue in td)
{
    Console.WriteLine(timePhasedValue.Value);
}
```

### См. также

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


