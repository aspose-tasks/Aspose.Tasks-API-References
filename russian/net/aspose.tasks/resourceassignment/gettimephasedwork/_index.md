---
title: "ResourceAssignment.GetTimephasedWork"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ResourceAssignment. Получает объём фазированной работы для указанного интервала даты и времени."
type: docs
weight: 730
url: /ru/net/aspose.tasks/resourceassignment/gettimephasedwork/
---
## GetTimephasedWork(DateTime, DateTime, TimephasedDataType) {#gettimephasedwork_1}

Получает количество timephased‑работы за указанный интервал дат и времени.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end, 
    TimephasedDataType timephasedDataType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| start | DateTime | Начало интервала даты и времени. |
| end | DateTime | Конец интервала даты и времени. |
| timephasedDataType | TimephasedDataType | Тип фазированных данных, которые следует использовать. |

## Примеры

Показывает, как вычислить работу назначения для произвольного интервала даты и времени.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var assignment = project.ResourceAssignments.GetByUid(2);

// Вывести работу назначения по каждому часу.
for (DateTime hour = assignment.Start; hour <= assignment.Finish; hour = hour.AddHours(1))
{
    var work = assignment.GetTimephasedWork(hour, hour.AddHours(1), TimephasedDataType.AssignmentWork);
    Console.WriteLine("{0} : {1:N2}", hour, work.TotalHours);
}
```

### См. также

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedWork(DateTime, DateTime) {#gettimephasedwork}

Получает количество timephased‑работы за указанный интервал дат и времени.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| start | DateTime | Начало интервала даты и времени. |
| end | DateTime | Конец интервала даты и времени. |

### См. также

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


