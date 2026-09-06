---
title: "الفئة TasksReadingException"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.TasksReadingException. تمثل نوع الاستثناء الداخلي القياسي للقراءة"
type: docs
weight: 2540
url: /ar/net/aspose.tasks/tasksreadingexception/
---
## TasksReadingException class

يمثّل نوع استثناء القراءة الداخلي القياسي.

```csharp
public class TasksReadingException : TasksLoggedException
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [LogText](../../aspose.tasks/tasksloggedexception/logtext/) { get; } | يحصل على معلومات تسجيل الاستثناء. |
| [Operation](../../aspose.tasks/tasksloggedexception/operation/) { get; } | يحصل على معلومات عملية الاستثناء. |

## الأمثلة

يعرض كيفية التعامل مع استثناءات قراءة/كتابة المشروع.

```csharp
try
{
    var project = new Project(DataDir + "project.mpp");
    project.Save(OutDir + "HandleExceptions_out.mpp", SaveFileFormat.Mpp);
}
catch (TasksReadingException ex)
{
    Console.WriteLine("Message: ");
    Console.WriteLine(ex.Message);
    Console.WriteLine("Log: ");
    Console.WriteLine(ex.LogText);
    if (ex.InnerException != null)
    {
        Console.WriteLine("Inner exception message: ");
        Console.WriteLine(ex.InnerException.Message);
    }
}
```

### انظر أيضًا

* class [TasksLoggedException](../tasksloggedexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


