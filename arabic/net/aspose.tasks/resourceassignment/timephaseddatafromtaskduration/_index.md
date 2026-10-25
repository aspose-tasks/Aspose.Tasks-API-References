---
title: "ResourceAssignment.TimephasedDataFromTaskDuration"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ResourceAssignment. تُنشئ قائمة من البيانات الزمنية المرحلية بناءً على مدة المهمة وتاريخ البدء المجدول"
type: docs
weight: 780
url: /ar/net/aspose.tasks/resourceassignment/timephaseddatafromtaskduration/
---
## ResourceAssignment.TimephasedDataFromTaskDuration method

ينشئ قائمة بالبيانات المتدرجة زمنياً بناءً على مدة المهمة وتاريخ البدء المجدول.

```csharp
public void TimephasedDataFromTaskDuration(Calendar calendar)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| تقويم | Calendar | التقويم المستخدم لإنشاء البيانات الزمنية المرحلية منه. |

## الأمثلة

يوضح كيفية إضافة تقسيم لمهمة.

```csharp
var project = new Project();

// احصل على تقويم قياسي
var calendar = project.Get(Prj.Calendar);

// ضبط إعدادات تقويم المشروع
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 4, 21, 17, 0, 0));

// إضافة مهمة جديدة إلى المهمة الجذرية
var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Duration, project.GetDuration(3));

// إنشاء تعيين مورد جديد وإنشاء بيانات زمنية مرحلية
var assignment = project.ResourceAssignments.Add(task, null);
assignment.TimephasedDataFromTaskDuration(calendar);

// قسّم المهمة إلى 3 أجزاء.
// قدّم وسيطات تاريخ البدء وتاريخ الانتهاء إلى طريقة SplitTask التي ستُستخدم للتقسيم
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 16, 17, 0, 0), calendar);
assignment.SplitTask(new DateTime(2000, 3, 18, 8, 0, 0), new DateTime(2000, 3, 18, 17, 0, 0), calendar);
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

project.Save(OutDir + "CreateSplitTasks_out.xml", SaveFileFormat.Xml);
```

### انظر أيضًا

* class [Calendar](../../calendar/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


