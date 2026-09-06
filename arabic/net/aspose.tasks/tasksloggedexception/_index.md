---
title: "الفئة TasksLoggedException"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.TasksLoggedException. تمثل نوع الاستثناء الداخلي القياسي"
type: docs
weight: 2530
url: /ar/net/aspose.tasks/tasksloggedexception/
---
## TasksLoggedException class

يمثّل نوع الاستثناء الداخلي القياسي.

```csharp
public class TasksLoggedException : ApplicationException
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | يحصل على معلومات تسجيل الاستثناء. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | يحصل على معلومات عملية الاستثناء. |

## الأمثلة

يظهر كيفية قراءة نص السجل ونوع الاستثناء للتحقق من المشكلات مع تصدير MPP.

```csharp
try
{
    var project = new Project(DataDir + "PrintTaskWritingException.mpp");

    // تصدير المشروع كملف MPP
    project.Save(OutDir + "PrintTaskWritingException_out.MPP", SaveFileFormat.Mpp);
}
catch (TasksWritingException ex)
{
    Console.WriteLine("Exception Operation: " + ex.Operation);
    Console.WriteLine("Exception Log Text: ");
    Console.WriteLine(ex.LogText);
}
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


