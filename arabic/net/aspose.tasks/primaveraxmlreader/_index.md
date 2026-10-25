---
title: "الفئة PrimaveraXmlReader"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.PrimaveraXmlReader. تمثل قارئًا يسمح باستخراج معرفات المشروع (UIDs) من ملف Primavera Xml"
type: docs
weight: 1400
url: /ar/net/aspose.tasks/primaveraxmlreader/
---
## PrimaveraXmlReader class

يمثل قارئًا يسمح باستخراج معرفات المشروع (UIDs) من ملف Primavera Xml.

```csharp
public class PrimaveraXmlReader : PrimaveraBaseReader
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor)(Stream) | يقوم بتهيئة نسخة جديدة من الفئة `PrimaveraXmlReader`. |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor_1)(string) | يقوم بتهيئة نسخة جديدة من الفئة `PrimaveraXmlReader`. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | إرجاع قائمة بكائنات معلومات مختصرة للمشروع. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | إرجاع قائمة بمعرفات المشاريع الفريدة. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | يقوم بتحميل المشروع بالمعرف الفريد المحدد. |

## الأمثلة

يوضح كيفية فحص معلومات المشاريع القصيرة من ملف Primavera XML.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### انظر أيضًا

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


