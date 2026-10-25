---
title: "TaskCollection.Add"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة TaskCollection. تُضيف المهمة المحددة إلى نسخة من فئة TaskCollection. إذا كان ParentProject.CalculationMode هو None يجب على المستخدم استدعاء Project.Recalculate بعد استخدام هذه الطريقة. سيُعيد جدولة جميع تواريخ بدء/انتهاء مهام المشروع، يحدد تواريخ مبكرة/متأخرة، ويحسب الحقول التابعة مثل الفجوات (slacks) والعمل وتكاليف الحقول والمعرفات ومستويات المخطط. إذا كان ParentProject.CalculationMode هو Manual فإن الطريقة ستحسب فقط معرف المهمة ومستوى المخطط وأرقام المخطط تلقائيًا. إذا كان ParentProject.CalculationMode هو Automatic فإن الطريقة تُعيد جدولة جميع مهام المشروع تلقائيًا (تواريخ بدء/انتهاء، تحدد تواريخ مبكرة/متأخرة، تحسب الفجوات، العمل وتكاليف الحقول، تعيد حساب المعرفات ومستويات المخطط)."
type: docs
weight: 50
url: /ar/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

أضف المهمة المحددة إلى نسخة من الفئة [`TaskCollection`](../). إذا كان ParentProject.CalculationMode هو None يجب على المستخدم استدعاء Project.Recalculate() بعد استخدام هذه الطريقة (سيُعيد جدولة جميع مهام المشروع (تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة) ويحسب الحقول التابعة مثل الفجوات، والعمل، وتكاليف الحقول، والمعرفات ومستويات المخطط). إذا كان ParentProject.CalculationMode هو Manual فإن الطريقة ستحسب فقط معرف المهمة، ومستوى المخطط، وأرقام المخطط تلقائيًا. إذا كان ParentProject.CalculationMode هو Automatic فإن الطريقة تُعيد جدولة جميع مهام المشروع تلقائيًا (تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة، تحسب الفجوات، والعمل، وتكاليف الحقول، وتعيد حساب المعرفات ومستويات المخطط).

```csharp
public void Add(Task item)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| العنصر | مهمة | المهمة المحددة التي يجب إضافتها إلى مجموعة المهام هذه. |

## الأمثلة

يعرض كيفية نقل مهمة تحت أصل آخر.

```csharp
var project = new Project(DataDir + "MoveTask.mpp") { CalculationMode = CalculationMode.Automatic };

// احصل على المهام حسب المعرفات
var task = project.RootTask.Children.GetByUid(6);
var task2 = project.RootTask.Children.GetByUid(3);

// إضافة المهمة 6 إلى أصل آخر
task2.Children.Add(task);
```

### انظر أيضًا

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add() {#add}

يضيف مهمة جديدة إلى مجموعة مهام المشروع على نفس مستوى المخطط للمهمة الأخيرة.

```csharp
public Task Add()
```

### قيمة الإرجاع

يعيد النسخة المضافة حديثًا من الفئة [`Task`](../../task/).

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

---

## Add(string) {#add_2}

يضيف مهمة جديدة إلى مجموعة مهام الأطفال.

```csharp
public Task Add(string taskName)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| taskName | سلسلة | اسم المهمة المحدد. |

### قيمة الإرجاع

يعيد النسخة المضافة حديثًا من الفئة [`Task`](../../task/).

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

---

## Add(string, int) {#add_3}

يضيف مهمة متكررة جديدة إلى مجموعة مهام الأطفال.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| taskName | سلسلة | اسم المهمة المحدد. |
| beforeTaskId | Int32 | المعرف المحدد لمهمة سيتُدرج أمامها مهمة جديدة. |

### قيمة الإرجاع

يعيد مهمة تم إدراجها قبل مهمة ذات المعرف المحدد.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentOutOfRangeException | يتم رمي ArgumentOutOfRangeException إذا كان المعرف المحدد غير صالح كمُعرف مهمة. |

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

---

## Add(RecurringTaskParameters) {#add_1}

يدرج مهمة جديدة قبل مهمة ذات المعرف المحدد وعلى نفس مستوى المخطط.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| parameters | RecurringTaskParameters | المعلمات المحددة لإنشاء مهمة متكررة. |

### قيمة الإرجاع

يعيد النسخة المضافة حديثًا من الفئة [`Task`](../../task/).

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | يتم رمي الاستثناء إذا كانت المعلمات المحددة فارغة (null). |
| ArgumentException | يتم رمي الاستثناء إذا كانت المعلمات المحددة غير صالحة. |

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
* class [RecurringTaskParameters](../../recurringtaskparameters/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)


