---
title: "ResourceAssignment.MakeTPs"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ResourceAssignment. Генерирует список данных с фазированием во времени"
type: docs
weight: 740
url: /ru/net/aspose.tasks/resourceassignment/maketps/
---
## ResourceAssignment.MakeTPs method

Генерирует список time phased данных.

```csharp
public DateTime MakeTPs(DateTime start, TimeSpan time, Calendar calendar, 
    List<TimephasedData> list, bool isWorking, int type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| start | DateTime | Указанная дата начала. |
| time | TimeSpan | Указанное рабочее время. |
| календарь | Calendar | Указанный рабочий календарь. |
| list | List`1 | Список данных с фазированием во времени. |
| isWorking | Boolean | Указанный флаг, определяющий, являются ли данные с фазированием во времени рабочими или нет. |
| тип | Int32 | Указанный тип данных с фазированием во времени. |

### Возвращаемое значение

Максимальная дата из списка или дата начала, если список пуст.

## Примеры

Показывает, как генерировать ТП по параметрам.

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

### См. также

* class [Calendar](../../calendar/)
* class [TimephasedData](../../timephaseddata/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


