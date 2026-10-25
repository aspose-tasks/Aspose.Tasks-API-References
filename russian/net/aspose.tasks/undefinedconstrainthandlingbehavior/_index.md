---
title: "Перечисление UndefinedConstraintHandlingBehavior"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.UndefinedConstraintHandlingBehavior. Указывает поведение, используемое для обработки задач с неопределёнными ограничениями"
type: docs
weight: 2630
url: /ru/net/aspose.tasks/undefinedconstrainthandlingbehavior/
---
## UndefinedConstraintHandlingBehavior enumeration

Указывает поведение, используемое для обработки задач с неопределёнными ограничениями.

```csharp
public enum UndefinedConstraintHandlingBehavior
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Поведение по умолчанию при загрузке из формата XER. Никаких действий не выполняется. Тип ограничения задачи устанавливается в 'ConstraintType.Undefined'. |
| SubstituteWithStartNoEarlierThan | `1` | Ограничения типа 'ConstraintType.StartNoEarlierThan' и датой = Start добавляются для задач с ограничением 'Undefined'. |

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


