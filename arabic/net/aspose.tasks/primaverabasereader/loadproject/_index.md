---
title: "PrimaveraBaseReader.LoadProject"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة PrimaveraBaseReader. تُحمّل المشروع بالمعرف الفريد المحدد."
type: docs
weight: 30
url: /ar/net/aspose.tasks/primaverabasereader/loadproject/
---
## PrimaveraBaseReader.LoadProject method

يقوم بتحميل المشروع بالمعرف الفريد المحدد.

```csharp
public virtual Project LoadProject(int projectUid)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| projectUid | Int32 | المعرف الفريد للمشروع الذي سيتم تحميله. |

### قيمة الإرجاع

المشروع بالمعرف الفريد المحدد من ملف متعدد المشاريع المحدد. قيمة Null إذا لم يكن المشروع موجودًا.

## الأمثلة

يوضح كيفية تحميل مشروع من ملف Primavera XML عندما يكون معرف المشروع معروفًا.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "PrimaveraProject.xml");
var project = reader.LoadProject(3882);
Console.WriteLine(project.Name);
```

يوضح كيفية فحص معلومات المشاريع المختصرة من ملف Primavera XER.

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### انظر أيضًا

* class [Project](../../project/)
* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


