---
title: "TaskLinkCollection.Add"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة TaskLinkCollection. تُعيد مثيلاً من FinishStart TaskLink الذي تم إضافته إلى كائن TaskLinkCollection"
type: docs
weight: 40
url: /ar/net/aspose.tasks/tasklinkcollection/add/
---
## Add(Task, Task) {#add}

يعيد مثيلاً من Finish-Start [`TaskLink`](../../tasklink/) تم إضافته إلى كائن TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| pred | مهمة | مهمة سابقة. |
| succ | مهمة | مهمة لاحقة. |

### قيمة الإرجاع

مثيل رابط مهمة تم إضافته إلى هذا الكائن.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | إذا كان أي من مهام الإدخال يساوي null فسيتم رمي استثناء ArgumentNullException. |

## الأمثلة

يوضح كيفية العمل مع مجموعات روابط المهام.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// احصل على المهام
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// اربط المهام
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// اطبع الروابط بين المهام
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// حرّر الرابط عبر الوصول بالفهرس
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// احذف جميع روابط المهام
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### انظر أيضًا

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType) {#add_1}

يعيد مثيلاً من [`TaskLink`](../../tasklink/) تم إضافته إلى كائن TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| pred | مهمة | مهمة سابقة. |
| succ | مهمة | مهمة لاحقة. |
| linkType | TaskLinkType | نوع الرابط [`TaskLinkType`](../../tasklinktype/) |

### قيمة الإرجاع

مثيل رابط مهمة تم إضافته إلى هذا الكائن.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | إذا كان أي من مهام الإدخال يساوي null فسيتم رمي استثناء ArgumentNullException. |

## الأمثلة

يوضح كيفية العمل مع مجموعات روابط المهام.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// احصل على المهام
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// اربط المهام
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// اطبع الروابط بين المهام
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// حرّر الرابط عبر الوصول بالفهرس
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// احذف جميع روابط المهام
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### انظر أيضًا

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType, Duration) {#add_2}

يعيد مثيلاً من [`TaskLink`](../../tasklink/) تم إضافته إلى كائن TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType, Duration lag)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| pred | مهمة | مهمة سابقة. |
| succ | مهمة | مهمة لاحقة. |
| linkType | TaskLinkType | نوع الرابط [`TaskLinkType`](../../tasklinktype/) |
| lag | Duration | تأخير الرابط [`Duration`](../../duration/). |

### قيمة الإرجاع

رابط مهمة تم إضافته إلى هذا الكائن.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | إذا كان أي من مهام الإدخال يساوي null فسيتم رمي استثناء ArgumentNullException. |

## الأمثلة

يوضح كيفية العمل مع مجموعات روابط المهام.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// احصل على المهام
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// اربط المهام
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// اطبع الروابط بين المهام
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// حرّر الرابط عبر الوصول بالفهرس
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// احذف جميع روابط المهام
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### انظر أيضًا

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* struct [Duration](../../duration/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(TaskLink) {#add_3}

هذا هو تنفيذ النموذج الأولي لطريقة Add في ICollection، والذي يرمي فقط NotSupportedException

```csharp
public void Add(TaskLink item)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| العنصر | TaskLink | العنصر المراد إضافته. |

### انظر أيضًا

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


