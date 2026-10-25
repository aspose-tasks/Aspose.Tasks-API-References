---
title: "TaskCollection.ToList"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة TaskCollection. تحول كائن TaskCollection إلى قائمة من كائنات Task"
type: docs
weight: 120
url: /ar/net/aspose.tasks/taskcollection/tolist/
---
## TaskCollection.ToList method

تحول كائن TaskCollection إلى قائمة من كائنات [`Task`](../../task/)

```csharp
public List<Task> ToList()
```

### قيمة الإرجاع

يعيد قائمة تحتوي على مثيلات الفئة [`Task`](../../task/) لهذه المجموعة.

## الأمثلة

يظهر كيفية العمل مع مجموعات المهام.

```csharp
var project = new Project();

// مجموعة المهام ليست للقراءة فقط ويمكن توسيعها
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// إنشاء مهام
var task1 = project.RootTask.Children.Add();
task1.Set(Tsk.Name, "Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task1.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task3.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task3.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2", 2);
task2.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// طباعة مهام المشروع
Console.WriteLine("Count of tasks: " + project.RootTask.Children.Count);
foreach (var child in project.RootTask.Children)
{
    Console.WriteLine("Parent Project: " + project.RootTask.ParentProject.Get(Prj.Name));
    Console.WriteLine("Task name: " + child.Get(Tsk.Name));
    Console.WriteLine("Task start: " + child.Get(Tsk.Start));
    Console.WriteLine("Task duration: " + child.Get(Tsk.Duration));
    Console.WriteLine("Task finish: " + child.Get(Tsk.Finish));
    Console.WriteLine();
}

// يمكن أخذ مهمة من المجموعة بواسطة المعرف ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// أو بواسطة UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// يمكن أيضًا إضافة مهمة متكررة
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2020, 4, 13, 8, 0, 0),
                                                                               Finish = new DateTime(2021, 4, 13, 17, 0, 0)
                                                                           }
                                                 }
                     };

// يتم إرجاع المهمة الأولى في التسلسل
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// يمكن تحويل المجموعة إلى قائمة بسيطة
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### انظر أيضًا

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)


