---
title: "VbaProject.HelpFile"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية VbaProject. تحصّل على اسم ملف المساعدة"
type: docs
weight: 40
url: /ar/net/aspose.tasks/vbaproject/helpfile/
---
## VbaProject.HelpFile property

يحصل على اسم ملف المساعدة

```csharp
public string HelpFile { get; }
```

## الأمثلة

يعرض كيفية قراءة خصائص مشروع VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
```

### انظر أيضًا

* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


