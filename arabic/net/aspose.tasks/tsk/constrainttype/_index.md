---
title: "Tsk.ConstraintType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. يوفر خيارات لنوع القيد الذي يمكن تطبيقه لجدولة مهمة."
type: docs
weight: 210
url: /ar/net/aspose.tasks/tsk/constrainttype/
---
## Tsk.ConstraintType field

يوفر خيارات لنوع القيد الذي يمكن تطبيقه لجدولة مهمة.

```csharp
public static readonly Key<ConstraintType, TaskKey> ConstraintType;
```

## الأمثلة

يعرض كيفية الحصول/تعيين قيد لمهمة.

```csharp
var project = new Project(DataDir + "ConstraintAsLateAsPossible.mpp");

// تعيين القيد كأقصى تأخير ممكن للمهمة ذات المعرف 11
var newTask = project.RootTask.Children.GetById(11);
newTask.Set(Tsk.ConstraintType, ConstraintType.AsLateAsPossible);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// تحليل جميع المهام المجمعة
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.ConstraintType).ToString());
    Console.WriteLine(task.Get(Tsk.ConstraintDate).ToShortDateString() == "1/1/2000" ? "NA" : task.Get(Tsk.ConstraintDate).ToShortDateString());
}

SaveOptions options = new PdfSaveOptions
{
    StartDate = project.Get(Prj.StartDate),
    Timescale = Timescale.ThirdsOfMonths
};

project.Save(OutDir + "SetConstraintAsLateAsPossible_out.pdf", options);
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [ConstraintType](../../constrainttype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


