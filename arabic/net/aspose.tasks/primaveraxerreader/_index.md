---
title: "الفئة PrimaveraXerReader"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.PrimaveraXerReader. تمثل قارئًا لقراءة معرفات المشاريع (UIDs) من ملف Primavera XER."
type: docs
weight: 1390
url: /ar/net/aspose.tasks/primaveraxerreader/
---
## PrimaveraXerReader class

يمثل قارئًا لقراءة معرفات المشروع (UIDs) من ملف Primavera XER

```csharp
public sealed class PrimaveraXerReader : PrimaveraBaseReader
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PrimaveraXerReader](primaveraxerreader/#constructor)(Stream) | ينشئ مثيلًا جديدًا من الفئة `PrimaveraXerReader`. |
| [PrimaveraXerReader](primaveraxerreader/#constructor_1)(string) | ينشئ مثيلًا جديدًا من الفئة `PrimaveraXerReader`. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | إرجاع قائمة بكائنات معلومات مختصرة للمشروع. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | إرجاع قائمة بمعرفات المشاريع الفريدة. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | يقوم بتحميل المشروع بالمعرف الفريد المحدد. |

## الأمثلة

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

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


