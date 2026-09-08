---
title: "Перечисление TaskStartDateType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.TaskStartDateType. Указывает тип даты начала задачи"
type: docs
weight: 2450
url: /ru/net/aspose.tasks/taskstartdatetype/
---
## TaskStartDateType enumeration

Указывает тип даты начала задачи.

```csharp
public enum TaskStartDateType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Undefined | `-1` | Значение поля не было определено в оригинальном файле проекта. |
| ProjectStartDate | `0` | Дата начала проекта |
| CurrentDate | `1` | Текущая дата |

## Примечания

При экспорте в XML неопределённые значения будут удалены из результирующего XML.

## Примеры

Показывает, как установить дату начала задачи по умолчанию как 'CurrentDate'.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


