---
title: "Project.UpdateProjectWorkAsComplete"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Обновляет всю работу как завершённую до указанной даты для всего проекта"
type: docs
weight: 1270
url: /ru/net/aspose.tasks/project/updateprojectworkascomplete/
---
## UpdateProjectWorkAsComplete(DateTime, bool) {#updateprojectworkascomplete}

Обновляет всю работу как завершённую до указанной даты для всего проекта.

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| completeThrough | DateTime | Дата, до которой работа считается завершённой. |
| setZeroOrHundredPercentCompleteOnly | Boolean | Если установлено в true, обновляет только те задачи как 100% завершённые, у которых дата окончания раньше указанной даты завершения. В противном случае вычисляет значение процента завершения на основе запланированных дат начала и даты завершения. |

## Примеры

Показывает, как обновить проект и перенести незавершённую работу.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2014, 1, 27, 8, 0, 0));

// Добавить новые задачи
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Duration, task2.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task4 = project.RootTask.Children.Add("Task 4");
task4.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task5 = project.RootTask.Children.Add("Task 5");
task5.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));

// Добавить ссылки между задачами
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);
var link23 = project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);

// Задержка в один день
link23.LinkLag = 4800;
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart);

// Добавить новые задачи
var task6 = project.RootTask.Children.Add("Task 6");
var task7 = project.RootTask.Children.Add("Task 7");
task7.Set(Tsk.Duration, task7.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task8 = project.RootTask.Children.Add("Task 8");
task8.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task9 = project.RootTask.Children.Add("Task 9");
task9.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task10 = project.RootTask.Children.Add("Task 10");

// Добавить ссылки между задачами
project.TaskLinks.Add(task6, task7, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task7, task8, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task8, task9, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task9, task10, TaskLinkType.FinishToStart);
task6.Set(Tsk.IsManual, true);
task7.Set(Tsk.IsManual, true);
task8.Set(Tsk.IsManual, true);
task9.Set(Tsk.IsManual, true);
task10.Set(Tsk.IsManual, true);

// Сохранить проект до и после обновления работы как завершённой
project.Save(OutDir + "RescheduleUncompletedWork_not updated_out.xml", SaveFileFormat.Xml);

// Сохранить проект после обновления работы проекта как завершённой только для указанных задач
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false, new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_updated_out.xml", SaveFileFormat.Xml);

// Сохранить проект после обновления всей работы проекта как завершённой
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false);
project.Save(OutDir + "RescheduleUncompletedWork_updated_out.xml", SaveFileFormat.Xml);

// Сохранить проект после переноса незавершённой работы только для указанных задач
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 8, 8, 0, 0), new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_rescheduled_out.xml", SaveFileFormat.Xml);

// Сохранить проект после переноса незавершённой работы
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 7, 8, 0, 0));
project.Save(OutDir + "RescheduleUncompletedWork_rescheduled_out.xml", SaveFileFormat.Xml);
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## UpdateProjectWorkAsComplete(DateTime, bool, List&lt;Task&gt;) {#updateprojectworkascomplete_1}

Обновляет всю работу как завершённую до указанной даты для указанного списка задач.

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly, List<Task> taskCollection)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| completeThrough | DateTime | Дата, до которой работа считается завершённой. |
| setZeroOrHundredPercentCompleteOnly | Boolean | Если установлено в true, обновляет только те задачи как 100% завершённые, у которых дата окончания раньше указанной даты завершения. В противном случае вычисляет значение процента завершения на основе запланированных дат начала и даты завершения. |
| taskCollection | List`1 | List&lt;Task&gt; задач, для которых необходимо обновить работу. |

## Примеры

Показывает, как обновить проект и перенести незавершённую работу.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2014, 1, 27, 8, 0, 0));

// Добавить новые задачи
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Duration, task2.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task4 = project.RootTask.Children.Add("Task 4");
task4.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task5 = project.RootTask.Children.Add("Task 5");
task5.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));

// Добавить ссылки между задачами
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);
var link23 = project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);

// Задержка в один день
link23.LinkLag = 4800;
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart);

// Добавить новые задачи
var task6 = project.RootTask.Children.Add("Task 6");
var task7 = project.RootTask.Children.Add("Task 7");
task7.Set(Tsk.Duration, task7.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task8 = project.RootTask.Children.Add("Task 8");
task8.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task9 = project.RootTask.Children.Add("Task 9");
task9.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task10 = project.RootTask.Children.Add("Task 10");

// Добавить ссылки между задачами
project.TaskLinks.Add(task6, task7, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task7, task8, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task8, task9, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task9, task10, TaskLinkType.FinishToStart);
task6.Set(Tsk.IsManual, true);
task7.Set(Tsk.IsManual, true);
task8.Set(Tsk.IsManual, true);
task9.Set(Tsk.IsManual, true);
task10.Set(Tsk.IsManual, true);

// Сохранить проект до и после обновления работы как завершённой
project.Save(OutDir + "RescheduleUncompletedWork_not updated_out.xml", SaveFileFormat.Xml);

// Сохранить проект после обновления работы проекта как завершённой только для указанных задач
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false, new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_updated_out.xml", SaveFileFormat.Xml);

// Сохранить проект после обновления всей работы проекта как завершённой
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false);
project.Save(OutDir + "RescheduleUncompletedWork_updated_out.xml", SaveFileFormat.Xml);

// Сохранить проект после переноса незавершённой работы только для указанных задач
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 8, 8, 0, 0), new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_rescheduled_out.xml", SaveFileFormat.Xml);

// Сохранить проект после переноса незавершённой работы
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 7, 8, 0, 0));
project.Save(OutDir + "RescheduleUncompletedWork_rescheduled_out.xml", SaveFileFormat.Xml);
```

### См. также

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


