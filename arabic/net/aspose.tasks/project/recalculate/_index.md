---
title: "Project.Recalculate"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Project. يعيد جدولة جميع مهام المشروع ids مستويات المخطط تواريخ البدء/الانتهاء يحدد تواريخ مبكرة/متأخرة يحسب الفجوات العمل وحقول التكلفة"
type: docs
weight: 1150
url: /ar/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

يعيد جدولة جميع معرفات مهام المشروع، مستويات المخطط، تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة، يحسب الفجوات، حقول العمل والتكلفة.

```csharp
public void Recalculate()
```

## الأمثلة

يعرض كيفية إعادة جدولة المشروع من تاريخ البدء بدلاً من تاريخ الانتهاء.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, new DateTime(2014, 1, 1));

// الآن يتم حساب جميع تواريخ المهام (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish). للحصول على المسار الحرج نحتاج إلى حساب الفواصل (يمكن استدعاؤها في خيط منفصل، ولكن فقط بعد حساب جميع تواريخ البدء/الانتهاء المبكرة والمتأخرة).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

يعيد جدولة جميع معرفات مهام المشروع، مستويات المخطط، تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة، يحسب الفجوات، حقول العمل والتكلفة مع التحقق الاختياري.

```csharp
public void Recalculate(bool validate)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| validate | Boolean | إذا كان صحيحًا سيتم إجراء التحقق من إعادة الحساب. ما البيانات التي يتم التحقق منها: في الوقت الحالي يتم تنفيذ التحقق الأساسي من نطاقات تواريخ المهمة وروابط المهمة فقط. سيتم فحص نطاقات تواريخ المهمة (مثل ActualStart - ActualFinish، EarlyStart - EarlyFinish، إلخ) وكذلك تواريخ روابط المهمة مقابل معيار التاريخ الذي يكون فيه تاريخ البدء أقل أو يساوي تاريخ الانتهاء. إذا فشل أي من الشروط المذكورة أعلاه سيتم رمي الاستثناء [`RecalculationValidationException`](../../recalculationvalidationexception/). |

## الأمثلة

يعرض كيفية إعادة حساب المشروع مع التحقق اللاحق.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("t1");
task.Set(Tsk.CommitmentStart, new DateTime(2017, 6, 19, 8, 0, 0));
task.Set(Tsk.CommitmentFinish, new DateTime(2017, 6, 18, 17, 0, 0));

try
{
    // إعادة حساب المشروع مع التحقق اللاحق
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


