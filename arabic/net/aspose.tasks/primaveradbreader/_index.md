---
title: "الفئة PrimaveraDbReader"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.PrimaveraDbReader. تمثل قارئًا لقراءة معلومات المشروع من قاعدة بيانات Primavera."
type: docs
weight: 1350
url: /ar/net/aspose.tasks/primaveradbreader/
---
## PrimaveraDbReader class

يمثل قارئًا لقراءة معلومات المشروع من قاعدة بيانات Primavera

```csharp
public sealed class PrimaveraDbReader : PrimaveraBaseReader
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PrimaveraDbReader](primaveradbreader/)(PrimaveraDbSettings) | ينشئ مثيلًا جديدًا للفئة [`PrimaveraXerReader`](../primaveraxerreader/). |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | إرجاع قائمة بكائنات معلومات مختصرة للمشروع. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | إرجاع قائمة بمعرفات المشاريع الفريدة. |
| override [LoadProject](../../aspose.tasks/primaveradbreader/loadproject/)(int) | يقوم بتحميل المشروع بالمعرف الفريد المحدد. |

## الأمثلة

يظهر كيفية الحصول على معلومات مختصرة للمشاريع من قاعدة بيانات Primavera.

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### انظر أيضًا

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


