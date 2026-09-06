---
title: "TasksLoggedException.Operation"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية TasksLoggedException. تحصل على معلومات عملية الاستثناء"
type: docs
weight: 20
url: /ar/net/aspose.tasks/tasksloggedexception/operation/
---
## TasksLoggedException.Operation property

يحصل على معلومات عملية الاستثناء.

```csharp
public string Operation { get; }
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


