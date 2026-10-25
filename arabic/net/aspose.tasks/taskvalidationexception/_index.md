---
title: "الفئة TaskValidationException"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.TaskValidationException. تمثل استثناءً يُرمى عندما يتم العثور على أخطاء في مهام المشاريع بعد إعادة الحساب"
type: docs
weight: 2510
url: /ar/net/aspose.tasks/taskvalidationexception/
---
## TaskValidationException class

يمثّل استثناء يُرمى عندما تُكتشف أخطاء في مهام المشروع بعد إعادة الحساب.

```csharp
public class TaskValidationException : RecalculationValidationException
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Task](../../aspose.tasks/taskvalidationexception/task/) { get; } | يحصل على المهمة التي تسببت في الاستثناء. |

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

* class [RecalculationValidationException](../recalculationvalidationexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


