---
title: "Resource.GetTimephasedData"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Resource. Возвращает экземпляр класса TimephasedDataCollection для этого объекта с значениями TimephasedData в указанных начальной и конечной датах заданного типа TimephasedDataType"
type: docs
weight: 850
url: /ru/net/aspose.tasks/resource/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Возвращает экземпляр класса [`TimephasedDataCollection`](../../timephaseddatacollection/) для этого объекта с значениями [`TimephasedData`](../timephaseddata/) в указанных начальной и конечной датах заданного [`TimephasedDataType`](../../timephaseddatatype/).

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

Список [`TimephasedData`](../timephaseddata/).

## Примеры

Показывает, как читать данные с фазированием во времени для ресурсов работы/стоимости.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// Получить ресурс по его идентификатору
var resource = project.Resources.GetByUid(1);

// Вывести данные с фазированием во времени ресурса ResourceWork
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// Вывести данные с фазированием во времени ресурса ResourceCost
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### См. также

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Возвращает [`TimephasedDataCollection`](../../timephaseddatacollection/) для этого объекта с значениями [`TimephasedData`](../timephaseddata/) в указанных начальной и конечной датах.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| start | DateTime | Дата начала для данных с фазированием во времени. |
| end | DateTime | Дата окончания для данных с фазированием во времени. |

### Возвращаемое значение

Список [`TimephasedData`](../../timephaseddata/).

## Примеры

Показывает, как читать данные с фазированием во времени для ресурсов работы/стоимости.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// Получить ресурс по его идентификатору
var resource = project.Resources.GetByUid(1);

// Вывести данные с фазированием во времени ресурса ResourceWork
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// Вывести данные с фазированием во времени ресурса ResourceCost
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### См. также

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


