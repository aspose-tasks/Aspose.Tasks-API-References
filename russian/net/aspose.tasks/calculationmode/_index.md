---
title: "Перечисление CalculationMode"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.CalculationMode. Указывает режим расчёта проекта"
type: docs
weight: 210
url: /ru/net/aspose.tasks/calculationmode/
---
## CalculationMode enumeration

Указывает режим расчёта проекта.

```csharp
public enum CalculationMode
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | None. Даты и затраты проекта не пересчитываются в этом режиме. |
| Automatic | `1` | Automatic mode. Даты и затраты проекта пересчитываются при использовании этого режима. |
| Manual | `2` | Manual mode. В этом режиме пересчитываются только необходимые поля, например UID и ID объектов. |

## Примеры

Показывает, как использовать режим автоматического расчёта.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Automatic
};

// Установите дату начала проекта и добавьте новые задачи
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// Свяжите задачи
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// Проверьте, что даты были пересчитаны
Console.WriteLine("Task1 Start + 1 Equals Task2 Start : {0} ", task1.Get(Tsk.Start).AddDays(1).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish + 1 Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).AddDays(1).Equals(task2.Get(Tsk.Finish)));
Console.WriteLine("RootTask Finish Equals Task2 Finish : {0} ", task2.Get(Tsk.Finish).Equals(project.RootTask.Get(Tsk.Finish)));
Console.WriteLine("Project Finish Date Equals Task2 Finish : {0} ", task2.Get(Tsk.Finish).Equals(project.Get(Prj.FinishDate)));
```

Показывает, как использовать режим без расчёта (none).

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.None
};

// Добавьте новую задачу
var task = project.RootTask.Children.Add("Task");

// Обратите внимание, что даже идентификаторы не были рассчитаны            
Console.WriteLine("Task.Id Equals 0 : {0} ", task.Get(Tsk.Id).Equals(0));
Console.WriteLine("Task.OutlineLevel Equals 0 : {0} ", task.Get(Tsk.OutlineLevel).Equals(0));
Console.WriteLine("Task Start Equals DateTime.MinValue : {0} ", task.Get(Tsk.Start).Equals(DateTime.MinValue));
Console.WriteLine("Task Finish Equals DateTime.MinValue : {0} ", task.Get(Tsk.Finish).Equals(DateTime.MinValue));
Console.WriteLine("Task Duration Equals 0 mins : {0} ", task.Get(Tsk.Duration).ToString().Equals("0 mins"));

// Установите свойство duration
task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));
Console.WriteLine("Task Duration Equals 2 days : {0} ", task.Get(Tsk.Duration).ToString().Equals("2 days"));
Console.WriteLine("Task Start Equals DateTime.MinValue  : {0} ", task.Get(Tsk.Start).Equals(DateTime.MinValue));
Console.WriteLine("Task Finish Equals DateTime.MinValue  : {0} ", task.Get(Tsk.Finish).Equals(DateTime.MinValue));
```

Показывает, как использовать режим ручного расчёта.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Manual
};

// Установите дату начала проекта и добавьте новые задачи
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// Необходимые свойства установлены в режиме ручного расчёта
Console.WriteLine("Task1.Id Equals 1 : {0} ", task1.Get(Tsk.Id).Equals(1));
Console.WriteLine("Task1 OutlineLevel Equals 1 : {0} ", task1.Get(Tsk.OutlineLevel).Equals(1));
Console.WriteLine("Task1 Start Equals 15/04/2015 08:00 AM : {0} ", task1.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task1 Finish Equals 15/04/2015 05:00 PM : {0} ", task1.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task1 Duration Equals 1 day : {0} ", task1.Get(Tsk.Duration).ToString().Equals("1 day"));
Console.WriteLine("Task2 Start Equals 15/04/2015 08:00 AM : {0} ", task2.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task2 Finish Equals 15/04/2015 05:00 PM : {0} ", task2.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task2 Duration Equals 1 day : {0} ", task2.Get(Tsk.Duration).ToString().Equals("1 day"));

// Когда мы связываем две задачи вместе, их даты не пересчитываются в режиме ручного расчёта
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// Начало задачи 2 не было изменено
Console.WriteLine("Task1 Start Equals Task2 Start : {0} ", task1.Get(Tsk.Start).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).Equals(task2.Get(Tsk.Finish)));
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


