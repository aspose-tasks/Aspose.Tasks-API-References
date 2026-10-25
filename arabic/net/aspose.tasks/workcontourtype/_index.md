---
title: "التعداد WorkContourType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.WorkContourType. يحدد شكل العمل"
type: docs
weight: 3610
url: /ar/net/aspose.tasks/workcontourtype/
---
## WorkContourType enumeration

يحدد مخطط العمل.

```csharp
public enum WorkContourType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Undefined | `-1` | القيمة لم تُعرّف في ملف المشروع الأصلي. |
| Flat | `0` | شكل عمل مسطح. |
| BackLoaded | `1` | شكل عمل محمل من الخلف. |
| FrontLoaded | `2` | شكل عمل محمل من الأمام. |
| DoublePeak | `3` | شكل عمل مزدوج القمة. |
| EarlyPeak | `4` | شكل عمل قمة مبكرة. |
| LatePeak | `5` | شكل عمل قمة متأخرة. |
| Bell | `6` | شكل عمل على شكل جرس. |
| Turtle | `7` | شكل عمل على شكل سلحفاة. |
| Contoured | `8` | مخطط عمل مخصص. |

## ملاحظات

أثناء التصدير إلى XML سيتم حذف القيم غير المعرفة من XML الناتج.

## الأمثلة

يظهر كيفية تعيين مخططات بيانات زمنية مختلفة لتخصيصات الموارد.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 1, 3, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 1, 7, 17, 0, 0));

// إضافة مهمة
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task.Set(Tsk.Finish, new DateTime(2000, 1, 3, 17, 0, 0));

var resource = project.Resources.Add("Resource");

// إضافة تخصيص مورد
var resourceAssignment = project.ResourceAssignments.Add(task, resource);
resourceAssignment.Set(Asn.Start, new DateTime(2000, 1, 3, 8, 0, 0));
resourceAssignment.Set(Asn.Work, project.GetWork(8));
resourceAssignment.Set(Asn.Finish, new DateTime(2000, 1, 3, 17, 0, 0));

// المخطط المسطح هو المخطط الافتراضي
Console.WriteLine("Flat contour");

var collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// تغيير المخطط
Console.WriteLine("Turtle contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.Turtle);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// تغيير المخطط
Console.WriteLine("BackLoaded contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.BackLoaded);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// تغيير المخطط
Console.WriteLine("FrontLoaded contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.FrontLoaded);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// تغيير المخطط
Console.WriteLine("Bell contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.Bell);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// تغيير المخطط
Console.WriteLine("EarlyPeak contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.EarlyPeak);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// تغيير المخطط
Console.WriteLine("LatePeak contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.LatePeak);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}

// تغيير المخطط
Console.WriteLine("DoublePeak contour");
resourceAssignment.Set(Asn.WorkContour, WorkContourType.DoublePeak);
collection = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate));
foreach (var td in collection)
{
    Console.WriteLine(td.Start.ToShortDateString() + " " + td.Value);
}
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


