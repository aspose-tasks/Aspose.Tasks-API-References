---
title: "ResourceAssignment.SplitTask"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ResourceAssignment. Делит задачу на две части"
type: docs
weight: 770
url: /ru/net/aspose.tasks/resourceassignment/splittask/
---
## ResourceAssignment.SplitTask method

Разделяет задачу на две части.

```csharp
public void SplitTask(DateTime start, DateTime finish, Calendar calendar)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| start | DateTime | Начало прерывания работы, на основе которого происходит разбиение. |
| завершение | DateTime | Конец прерывания работы, на основе которого происходит разбиение. |
| календарь | Calendar | Календарь, на основе которого происходит разбиение. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException | Выбрасывает исключение, когда дата начала меньше даты начала назначения. |
| ArgumentOutOfRangeException | Выбрасывает исключение, когда дата завершения больше даты завершения назначения. |

## Примеры

Показывает, как добавить разбиение для задачи.

```csharp
var project = new Project();

// Получить стандартный календарь
var calendar = project.Get(Prj.Calendar);

// Установить настройки календаря проекта
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 4, 21, 17, 0, 0));

// Добавить новую задачу к корневой задаче
var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Duration, project.GetDuration(3));

// Создать новое назначение ресурса и сгенерировать данные с разбивкой по времени
var assignment = project.ResourceAssignments.Add(task, null);
assignment.TimephasedDataFromTaskDuration(calendar);

// Разделить задачу на 3 части.
// Укажите аргументы даты начала и даты завершения для метода SplitTask, которые будут использованы для разбиения
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 16, 17, 0, 0), calendar);
assignment.SplitTask(new DateTime(2000, 3, 18, 8, 0, 0), new DateTime(2000, 3, 18, 17, 0, 0), calendar);
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

project.Save(OutDir + "CreateSplitTasks_out.xml", SaveFileFormat.Xml);
```

### См. также

* class [Calendar](../../calendar/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


