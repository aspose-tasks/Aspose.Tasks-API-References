---
title: "Task.GetTimephasedData"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Task. Возвращает объект TimephasedDataCollection со значениями TimephasedData в заданных начальной и конечной датах указанного типа timephased data."
type: docs
weight: 1360
url: /ru/net/aspose.tasks/task/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Возвращает объект [`TimephasedDataCollection`](../../timephaseddatacollection/) с значениями [`TimephasedData`](../timephaseddata/) в указанных начальной и конечной датах указанного типа time-phased data.

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

Объект [`TimephasedDataCollection`](../../timephaseddatacollection/) с значениями [`TimephasedData`](../timephaseddata/) в указанных начальной и конечной датах указанного типа timephased data.

## Примеры

Показывает, как получить timephased data (с определённым типом) задачи.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate).AddDays(2), TimephasedDataType.TaskBaselineWork)
    .ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### См. также

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Возвращает объект [`TimephasedDataCollection`](../../timephaseddatacollection/) с значениями [`TimephasedData`](../timephaseddata/) в указанных начальной и конечной датах.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| start | DateTime | Дата начала для данных с фазированием во времени. |
| end | DateTime | Дата окончания для данных с фазированием во времени. |

### Возвращаемое значение

Список [`TimephasedData`](../../timephaseddata/) для заполнения.

## Примеры

Показывает, как получить временно-фазовые данные (типа TaskWork) задачи.

```csharp
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)).ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### См. также

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


