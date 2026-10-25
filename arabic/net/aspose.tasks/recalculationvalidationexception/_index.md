---
title: "Class RecalculationValidationException"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.RecalculationValidationException class. يمثل استثناءً يُرمى عندما يتم العثور على أخطاء في المشروع بعد إعادة الحساب"
type: docs
weight: 1680
url: /ar/net/aspose.tasks/recalculationvalidationexception/
---
## RecalculationValidationException class

يمثل استثناءً يتم إلقاؤه عندما يتم العثور على أخطاء في المشروع بعد إعادة الحساب.

```csharp
public abstract class RecalculationValidationException : ValidationException
```

## الأمثلة

يعرض تحت أي ظروف يمكن رمي الاستثناء &lt;see cref=\"TaskValidationException\" /&gt;.

```csharp
try
{
    var project = new Project { CalculationMode = CalculationMode.None };
    var task = project.RootTask.Children.Add("Task");

    // تم تعيين تواريخ غير صحيحة عن طريق الخطأ
    task.Set(Tsk.Start, new DateTime(2017, 6, 19, 8, 0, 0));
    task.Set(Tsk.Duration, project.GetDuration(1));
    task.Set(Tsk.Finish, new DateTime(2017, 6, 18, 17, 0, 0));

    // تشغيل إعادة حساب المشروع مع علامة لتشغيل التحقق
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### انظر أيضًا

* class [ValidationException](../validationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


