---
title: "Перечисление TaskStatus"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.TaskStatus. Указывает статус задачи"
type: docs
weight: 2460
url: /ru/net/aspose.tasks/taskstatus/
---
## TaskStatus enumeration

Указывает статус задачи.

```csharp
public enum TaskStatus
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Undefined | `-1` | Неопределённый статус задачи. |
| Complete | `0` | Задача выполнена на 100 процентов. |
| OnSchedule | `1` | Задача находится в графике, если кумулятивный процент выполнения по фазам времени распределён как минимум до дня, предшествующего дате статуса. |
| Late | `2` | Задача просрочена, если кумулятивный процент выполнения по фазам времени не достигает полуночи дня, предшествующего дате статуса. |
| Future | `3` | Статус задачи 'Future' устанавливается, когда дата начала задачи позже даты статуса. |

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


