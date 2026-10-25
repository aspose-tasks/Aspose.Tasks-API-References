---
title: "الفئة TasksWritingException"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.TasksWritingException. تمثل نوع الاستثناء الداخلي القياسي للكتابة"
type: docs
weight: 2560
url: /ar/net/aspose.tasks/taskswritingexception/
---
## TasksWritingException class

يمثّل نوع استثناء الكتابة الداخلي القياسي.

```csharp
public class TasksWritingException : TasksLoggedException
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

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


