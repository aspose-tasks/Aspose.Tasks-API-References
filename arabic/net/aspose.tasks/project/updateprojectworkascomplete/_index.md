---
title: "Project.UpdateProjectWorkAsComplete"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Project. تقوم بتحديث كل العمل كمنجز حتى تاريخ محدد لكامل المشروع"
type: docs
weight: 1270
url: /ar/net/aspose.tasks/project/updateprojectworkascomplete/
---
## UpdateProjectWorkAsComplete(DateTime, bool) {#updateprojectworkascomplete}

يحدّث جميع الأعمال كمنجزة حتى تاريخ محدد لكامل المشروع.

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| completeThrough | DateTime | التاريخ لتحديث العمل كمنجز حتى. |
| setZeroOrHundredPercentCompleteOnly | Boolean | إذا تم تعيينه إلى true، يتم تحديث تلك المهام فقط كمنجزة بنسبة 100% التي تاريخ انتهائها قبل تاريخ الإكمال المحدد. وإلا، يتم حساب قيمة النسبة المكتملة بناءً على تاريخ البدء المجدول وتواريخ الإكمال. |

## الأمثلة

يُظهر كيفية تحديث المشروع وإعادة جدولة العمل غير المكتمل.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2014, 1, 27, 8, 0, 0));

// إضافة مهام جديدة
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Duration, task2.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task4 = project.RootTask.Children.Add("Task 4");
task4.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task5 = project.RootTask.Children.Add("Task 5");
task5.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));

// إضافة روابط بين المهام
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);
var link23 = project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);

// تأخير يوم واحد
link23.LinkLag = 4800;
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart);

// إضافة مهام جديدة
var task6 = project.RootTask.Children.Add("Task 6");
var task7 = project.RootTask.Children.Add("Task 7");
task7.Set(Tsk.Duration, task7.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task8 = project.RootTask.Children.Add("Task 8");
task8.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task9 = project.RootTask.Children.Add("Task 9");
task9.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task10 = project.RootTask.Children.Add("Task 10");

// إضافة روابط بين المهام
project.TaskLinks.Add(task6, task7, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task7, task8, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task8, task9, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task9, task10, TaskLinkType.FinishToStart);
task6.Set(Tsk.IsManual, true);
task7.Set(Tsk.IsManual, true);
task8.Set(Tsk.IsManual, true);
task9.Set(Tsk.IsManual, true);
task10.Set(Tsk.IsManual, true);

// احفظ المشروع قبل وبعد تحديث العمل كمنجز
project.Save(OutDir + "RescheduleUncompletedWork_not updated_out.xml", SaveFileFormat.Xml);

// حفظ المشروع بعد تحديث عمل المشروع كمنتهي فقط للمهام المحددة
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false, new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_updated_out.xml", SaveFileFormat.Xml);

// حفظ المشروع بعد تحديث جميع أعمال المشروع كمنتهي
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false);
project.Save(OutDir + "RescheduleUncompletedWork_updated_out.xml", SaveFileFormat.Xml);

// حفظ المشروع بعد إعادة جدولة العمل غير المكتمل فقط للمهام المحددة
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 8, 8, 0, 0), new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_rescheduled_out.xml", SaveFileFormat.Xml);

// حفظ المشروع بعد إعادة جدولة العمل غير المكتمل
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 7, 8, 0, 0));
project.Save(OutDir + "RescheduleUncompletedWork_rescheduled_out.xml", SaveFileFormat.Xml);
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## UpdateProjectWorkAsComplete(DateTime, bool, List&lt;Task&gt;) {#updateprojectworkascomplete_1}

يحدّث جميع الأعمال كمنجزة حتى تاريخ محدد للقائمة المحددة من المهام.

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly, List<Task> taskCollection)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| completeThrough | DateTime | التاريخ لتحديث العمل كمنجز حتى. |
| setZeroOrHundredPercentCompleteOnly | Boolean | إذا تم تعيينه إلى true، يتم تحديث تلك المهام فقط كمنجزة بنسبة 100% التي تاريخ انتهائها قبل تاريخ الإكمال المحدد. وإلا، يتم حساب قيمة النسبة المكتملة بناءً على تاريخ البدء المجدول وتواريخ الإكمال. |
| taskCollection | List`1 | قائمة&lt;Task&gt; للمهام التي سيتم تحديث العمل لها. |

## الأمثلة

يُظهر كيفية تحديث المشروع وإعادة جدولة العمل غير المكتمل.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2014, 1, 27, 8, 0, 0));

// إضافة مهام جديدة
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Duration, task2.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task4 = project.RootTask.Children.Add("Task 4");
task4.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task5 = project.RootTask.Children.Add("Task 5");
task5.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));

// إضافة روابط بين المهام
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);
var link23 = project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);

// تأخير يوم واحد
link23.LinkLag = 4800;
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart);

// إضافة مهام جديدة
var task6 = project.RootTask.Children.Add("Task 6");
var task7 = project.RootTask.Children.Add("Task 7");
task7.Set(Tsk.Duration, task7.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task8 = project.RootTask.Children.Add("Task 8");
task8.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task9 = project.RootTask.Children.Add("Task 9");
task9.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task10 = project.RootTask.Children.Add("Task 10");

// إضافة روابط بين المهام
project.TaskLinks.Add(task6, task7, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task7, task8, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task8, task9, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task9, task10, TaskLinkType.FinishToStart);
task6.Set(Tsk.IsManual, true);
task7.Set(Tsk.IsManual, true);
task8.Set(Tsk.IsManual, true);
task9.Set(Tsk.IsManual, true);
task10.Set(Tsk.IsManual, true);

// احفظ المشروع قبل وبعد تحديث العمل كمنجز
project.Save(OutDir + "RescheduleUncompletedWork_not updated_out.xml", SaveFileFormat.Xml);

// حفظ المشروع بعد تحديث عمل المشروع كمنتهي فقط للمهام المحددة
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false, new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_updated_out.xml", SaveFileFormat.Xml);

// حفظ المشروع بعد تحديث جميع أعمال المشروع كمنتهي
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false);
project.Save(OutDir + "RescheduleUncompletedWork_updated_out.xml", SaveFileFormat.Xml);

// حفظ المشروع بعد إعادة جدولة العمل غير المكتمل فقط للمهام المحددة
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 8, 8, 0, 0), new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_rescheduled_out.xml", SaveFileFormat.Xml);

// حفظ المشروع بعد إعادة جدولة العمل غير المكتمل
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 7, 8, 0, 0));
project.Save(OutDir + "RescheduleUncompletedWork_rescheduled_out.xml", SaveFileFormat.Xml);
```

### انظر أيضًا

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


