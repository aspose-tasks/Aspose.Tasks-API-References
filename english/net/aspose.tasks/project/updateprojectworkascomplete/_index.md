---
title: Project.UpdateProjectWorkAsComplete
second_title: Aspose.Tasks for .NET API Reference
description: Project method. Updates all work as complete through a specified date for the entire project
type: docs
weight: 1270
url: /net/aspose.tasks/project/updateprojectworkascomplete/
---
## UpdateProjectWorkAsComplete(DateTime, bool) {#updateprojectworkascomplete}

Updates all work as complete through a specified date for the entire project.

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly)
```

| Parameter | Type | Description |
| --- | --- | --- |
| completeThrough | DateTime | The date to update work as completed through. |
| setZeroOrHundredPercentCompleteOnly | Boolean | If set to true updates only those tasks as 100% complete whose finish date is before specified complete-through date. Otherwise, calculates a percentage complete value based on scheduled start and complete-through dates. |

## Examples

Shows how to update the project and reschedule uncompleted work.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2014, 1, 27, 8, 0, 0));

// Add new tasks
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Duration, task2.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task4 = project.RootTask.Children.Add("Task 4");
task4.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task5 = project.RootTask.Children.Add("Task 5");
task5.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));

// Add links between tasks
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);
var link23 = project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);

// One day lag
link23.LinkLag = 4800;
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart);

// Add new tasks
var task6 = project.RootTask.Children.Add("Task 6");
var task7 = project.RootTask.Children.Add("Task 7");
task7.Set(Tsk.Duration, task7.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task8 = project.RootTask.Children.Add("Task 8");
task8.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task9 = project.RootTask.Children.Add("Task 9");
task9.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task10 = project.RootTask.Children.Add("Task 10");

// Add links between tasks
project.TaskLinks.Add(task6, task7, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task7, task8, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task8, task9, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task9, task10, TaskLinkType.FinishToStart);
task6.Set(Tsk.IsManual, true);
task7.Set(Tsk.IsManual, true);
task8.Set(Tsk.IsManual, true);
task9.Set(Tsk.IsManual, true);
task10.Set(Tsk.IsManual, true);

// Save project before and after updating work as completed 
project.Save(OutDir + "RescheduleUncompletedWork_not updated_out.xml", SaveFileFormat.Xml);

// Save project after updating project work as complete only for specified tasks
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false, new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_updated_out.xml", SaveFileFormat.Xml);

// Save project after updating all project work as complete
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false);
project.Save(OutDir + "RescheduleUncompletedWork_updated_out.xml", SaveFileFormat.Xml);

// Save project after rescheduling uncompleted work only for specified tasks
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 8, 8, 0, 0), new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_rescheduled_out.xml", SaveFileFormat.Xml);

// Save project after rescheduling uncompleted work
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 7, 8, 0, 0));
project.Save(OutDir + "RescheduleUncompletedWork_rescheduled_out.xml", SaveFileFormat.Xml);
```

### See Also

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## UpdateProjectWorkAsComplete(DateTime, bool, List&lt;Task&gt;) {#updateprojectworkascomplete_1}

Updates all work as complete through a specified date for the specified list of tasks.

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly, List<Task> taskCollection)
```

| Parameter | Type | Description |
| --- | --- | --- |
| completeThrough | DateTime | The date to update work as completed through. |
| setZeroOrHundredPercentCompleteOnly | Boolean | If set to true updates only those tasks as 100% complete whose finish date is before specified complete-through date. Otherwise, calculates a percentage complete value based on scheduled start and complete-through dates. |
| taskCollection | List`1 | List&lt;Task&gt; of tasks to update work for. |

## Examples

Shows how to update the project and reschedule uncompleted work.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2014, 1, 27, 8, 0, 0));

// Add new tasks
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Duration, task2.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task4 = project.RootTask.Children.Add("Task 4");
task4.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task5 = project.RootTask.Children.Add("Task 5");
task5.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));

// Add links between tasks
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);
var link23 = project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);

// One day lag
link23.LinkLag = 4800;
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart);

// Add new tasks
var task6 = project.RootTask.Children.Add("Task 6");
var task7 = project.RootTask.Children.Add("Task 7");
task7.Set(Tsk.Duration, task7.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task8 = project.RootTask.Children.Add("Task 8");
task8.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task9 = project.RootTask.Children.Add("Task 9");
task9.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task10 = project.RootTask.Children.Add("Task 10");

// Add links between tasks
project.TaskLinks.Add(task6, task7, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task7, task8, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task8, task9, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task9, task10, TaskLinkType.FinishToStart);
task6.Set(Tsk.IsManual, true);
task7.Set(Tsk.IsManual, true);
task8.Set(Tsk.IsManual, true);
task9.Set(Tsk.IsManual, true);
task10.Set(Tsk.IsManual, true);

// Save project before and after updating work as completed 
project.Save(OutDir + "RescheduleUncompletedWork_not updated_out.xml", SaveFileFormat.Xml);

// Save project after updating project work as complete only for specified tasks
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false, new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_updated_out.xml", SaveFileFormat.Xml);

// Save project after updating all project work as complete
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false);
project.Save(OutDir + "RescheduleUncompletedWork_updated_out.xml", SaveFileFormat.Xml);

// Save project after rescheduling uncompleted work only for specified tasks
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 8, 8, 0, 0), new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_rescheduled_out.xml", SaveFileFormat.Xml);

// Save project after rescheduling uncompleted work
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 7, 8, 0, 0));
project.Save(OutDir + "RescheduleUncompletedWork_rescheduled_out.xml", SaveFileFormat.Xml);
```

### See Also

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


