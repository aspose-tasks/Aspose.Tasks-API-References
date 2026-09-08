---
title: "Prj.DefaultTaskEVMethod"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Метод оценки заработанной стоимости по умолчанию для задач"
type: docs
weight: 280
url: /ru/net/aspose.tasks/prj/defaulttaskevmethod/
---
## Prj.DefaultTaskEVMethod field

Метод расчёта заработанной стоимости по умолчанию для задач.

```csharp
public static readonly Key<EarnedValueMethodType, PrjKey> DefaultTaskEVMethod;
```

## Примеры

Показывает, как прочитать свойства проекта по умолчанию.

```csharp
var project = new Project(DataDir + "DefaultProperties.mpp");

// Установить свойства по умолчанию
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, DateTime.Now);
project.Set(Prj.DefaultStartTime, project.Get(Prj.StartDate));
project.Set(Prj.DefaultTaskType, TaskType.FixedDuration);
project.Set(Prj.DefaultStandardRate, 15);
project.Set(Prj.DefaultOvertimeRate, 12);
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
project.Set(Prj.DefaultFixedCostAccrual, CostAccrualType.Prorated);

// Отобразить свойства по умолчанию
Console.WriteLine("New Task Default Start: " + project.Get(Prj.DefaultStartTime).ToShortDateString());
Console.WriteLine("New Task Default Type: " + project.Get(Prj.DefaultTaskType));
Console.WriteLine("Resource Default Standard Rate: " + project.Get(Prj.DefaultStandardRate));
Console.WriteLine("Resource Default Overtime Rate: " + project.Get(Prj.DefaultOvertimeRate));
Console.WriteLine("Default Task EV Method: " + project.Get(Prj.DefaultTaskEVMethod));
Console.WriteLine("Default Cost Accrual: " + project.Get(Prj.DefaultFixedCostAccrual));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


