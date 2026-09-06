---
title: "فئة VbaProject"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.VbaProject. تمثل VbaProject"
type: docs
weight: 2860
url: /ar/net/aspose.tasks/vbaproject/
---
## VbaProject class

يمثل `VbaProject`.

```csharp
public class VbaProject
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CompilationArguments](../../aspose.tasks/vbaproject/compilationarguments/) { get; } | يحصل على وسائط التجميع الشرطية |
| [Description](../../aspose.tasks/vbaproject/description/) { get; } | يحصل على وصف المشروع. |
| [HelpContextId](../../aspose.tasks/vbaproject/helpcontextid/) { get; } | يحصل على معرف سياق مساعدة المشروع |
| [HelpFile](../../aspose.tasks/vbaproject/helpfile/) { get; } | يحصل على اسم ملف المساعدة |
| [Modules](../../aspose.tasks/vbaproject/modules/) { get; } | يحصل على مجموعة من [`VbaModuleCollection`](../vbamodulecollection/) |
| [Name](../../aspose.tasks/vbaproject/name/) { get; } | يحصل على اسم المشروع |
| [References](../../aspose.tasks/vbaproject/references/) { get; } | يحصل على مجموعة من [`VbaReferenceCollection`](../vbareferencecollection/) |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


