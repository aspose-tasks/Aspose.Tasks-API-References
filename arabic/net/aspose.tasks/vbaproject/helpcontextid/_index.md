---
title: "VbaProject.HelpContextId"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية VbaProject. يحصل على معرف سياق المساعدة للمشروع"
type: docs
weight: 30
url: /ar/net/aspose.tasks/vbaproject/helpcontextid/
---
## VbaProject.HelpContextId property

يحصل على معرف سياق مساعدة المشروع

```csharp
public int HelpContextId { get; }
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


