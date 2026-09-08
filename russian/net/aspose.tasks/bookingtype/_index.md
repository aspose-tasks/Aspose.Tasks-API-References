---
title: "Перечисление BookingType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.BookingType. Указывает тип бронирования ресурса"
type: docs
weight: 150
url: /ru/net/aspose.tasks/bookingtype/
---
## BookingType enumeration

Указывает тип бронирования ресурса.

```csharp
public enum BookingType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Undefined | `-1` | Указывает, что значение не было определено в оригинальном файле проекта. |
| Committed | `0` | Указывает тип бронирования «Committed». |
| Proposed | `1` | Указывает тип бронирования «Proposed». |

## Примечания

При экспорте в XML неопределённые значения будут удалены из результирующего XML.

## Примеры

Показывает, как читать/записывать свойство Asn.BookingType.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.BookingType, BookingType.Proposed);

Console.WriteLine("Booking Type: " + assignment.Get(Asn.BookingType));
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


