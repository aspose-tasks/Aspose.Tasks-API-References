---
title: "الفئة ValidationException"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.ValidationException. تمثل استثناءً يُرمى عندما يتم العثور على أخطاء أثناء التحقق من صحة الكيان"
type: docs
weight: 2790
url: /ar/net/aspose.tasks/validationexception/
---
## ValidationException class

يمثّل استثناء يُرمى عندما تُكتشف أخطاء أثناء التحقق من صحة الكيان.

```csharp
public class ValidationException : ApplicationException
```

## الأمثلة

يوضح كيفية التعامل مع &lt;see cref="ValidationException"/&gt; أثناء العمل مع مهام التكرار.

```csharp
try
{
    var project = new Project();
    var parameters = new RecurringTaskParameters { TaskName = "t1", Duration = project.GetDuration(1, TimeUnitType.Day), RecurrencePattern = null };
    project.RootTask.Children.Add(parameters);
}
catch (ValidationException ex)
{
    Console.WriteLine("Message: ");
    Console.WriteLine(ex.Message);
    if (ex.InnerException != null)
    {
        Console.WriteLine("Inner exception message: ");
        Console.WriteLine(ex.InnerException.Message);
    }
}
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


