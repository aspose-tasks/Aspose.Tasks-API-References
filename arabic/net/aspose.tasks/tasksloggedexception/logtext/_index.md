---
title: "TasksLoggedException.LogText"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية TasksLoggedException. تحصل على معلومات تسجيل الاستثناء"
type: docs
weight: 10
url: /ar/net/aspose.tasks/tasksloggedexception/logtext/
---
## TasksLoggedException.LogText property

يحصل على معلومات تسجيل الاستثناء.

```csharp
public string LogText { get; }
```

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

* class [TasksLoggedException](../)
* namespace [Aspose.Tasks](../../tasksloggedexception/)
* assembly [Aspose.Tasks](../../../)


