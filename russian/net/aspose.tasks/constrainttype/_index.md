---
title: Enum ConstraintType
second_title: Справочник по Aspose.Tasks для .NET API
description: Aspose.Tasks.ConstraintType перечисление. Указывает ограничение на дату начала или окончания задачи.
type: docs
weight: 330
url: /ru/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

Указывает ограничение на дату начала или окончания задачи.

```csharp
public enum ConstraintType
```

### Ценности

| Имя | Ценность | Описание |
| --- | --- | --- |
| Undefined | `-1` | Значение не было определено в исходном файле проекта. |
| AsSoonAsPossible | `0` | [`Start`](../tsk/start/) и[`Finish`](../tsk/finish/) даты[`Task`](../task/) запланированы ASAP по отношению к родительскому[`Start`](../tsk/start/) и[`Finish`](../tsk/finish/)даты и учитывая[`TaskLinks`](../project/tasklinks/) . |
| AsLateAsPossible | `1` | [`Start`](../tsk/start/) и[`Finish`](../tsk/finish/) даты[`Task`](../task/) запланированы ALAP по отношению к родительскому[`Start`](../tsk/start/) и[`Finish`](../tsk/finish/)даты и учитывая[`TaskLinks`](../project/tasklinks/) . |
| MustStartOn | `2` | Должен начаться с |
| MustFinishOn | `3` | Должен закончиться на |
| StartNoEarlierThan | `4` | Начать не ранее, чем |
| StartNoLaterThan | `5` | Начать не позднее, чем |
| FinishNoEarlierThan | `6` | Завершить не ранее |
| FinishNoLaterThan | `7` | Завершить не позже, чем |

### Примечания

При экспорте в XML неопределенные значения будут удалены из результирующего XML.

### Смотрите также

* пространство имен [Aspose.Tasks](../../aspose.tasks/)
* сборка [Aspose.Tasks](../../)


