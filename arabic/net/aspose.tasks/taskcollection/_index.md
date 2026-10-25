---
title: "الفئة TaskCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.TaskCollection. تمثل مجموعة من كائنات Task"
type: docs
weight: 2390
url: /ar/net/aspose.tasks/taskcollection/
---
## TaskCollection class

تمثل مجموعة من كائنات [`Task`](../task/).

```csharp
public class TaskCollection : IList<Task>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | يحصل على عدد الكائنات الموجودة في TaskCollection. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | يرجع العنصر عند الفهرس المحدد. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | يحصل على المشروع الأب لكائن TaskCollection. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | يضيف مهمة جديدة إلى مجموعة مهام المشروع على نفس مستوى المخطط للمهمة الأخيرة. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | يدرج مهمة جديدة قبل مهمة ذات المعرف المحدد وعلى نفس مستوى المخطط. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | يضيف مهمة جديدة إلى مجموعة مهام الأطفال. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | أضف المهمة المحددة إلى نسخة من الفئة `TaskCollection`. إذا كان ParentProject.CalculationMode هو None يجب على المستخدم استدعاء Project.Recalculate() بعد استخدام هذه الطريقة (سيعيد جدولة جميع مهام المشروع (تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة) ويحسب الحقول التابعة مثل الفجوات، والعمل، وتكاليف الحقول، والمعرفات ومستويات المخطط). إذا كان ParentProject.CalculationMode هو Manual فإن الطريقة ستحسب فقط معرف المهمة، ومستوى المخطط، وأرقام المخطط تلقائيًا. إذا كان ParentProject.CalculationMode هو Automatic فإن الطريقة تعيد جدولة جميع مهام المشروع تلقائيًا (تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة، يحسب الفجوات، والعمل، وتكاليف الحقول، يعيد حساب المعرفات ومستويات المخطط). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | يضيف مهمة متكررة جديدة إلى مجموعة مهام الأطفال. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | يتحقق مما إذا كانت المجموعة تحتوي على العنصر المحدد. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | يرجع مهمة بالمعرف المحدد Id يكون سلفها المهمة الأب لهذه المجموعة. |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | يرجع مهمة بالمعرف الفريد المحدد Uid يكون سلفها المهمة الأب لهذه المجموعة. |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | هذه هي تنفيذية النموذجية لطريقة Insert في IList، التي ترمي فقط NotSupportedException |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | هذه هي تنفيذية النموذجية لطريقة Remove في ICollection، التي ترمي فقط NotSupportedException |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | تحول كائن TaskCollection إلى قائمة من كائنات [`Task`](../task/). |

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

* class [Task](../task/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


