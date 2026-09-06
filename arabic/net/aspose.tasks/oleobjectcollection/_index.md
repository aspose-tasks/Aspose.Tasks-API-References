---
title: "الفئة OleObjectCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.OleObjectCollection. تمثل مجموعة تحتوي على نسخ من الفئة OleObject."
type: docs
weight: 1130
url: /ar/net/aspose.tasks/oleobjectcollection/
---
## OleObjectCollection class

تمثل مجموعة تحتوي على نسخ من الفئة [`OleObject`](../oleobject/).

```csharp
public sealed class OleObjectCollection : IList<OleObject>
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Clear](../../aspose.tasks/oleobjectcollection/clear/)() | يمسح المجموعة. من أجل حفظ هذه التغييرات يجب استدعاء project.Save مع new MPPSaveOptions { WriteViewData = true; } |
| [GetEnumerator](../../aspose.tasks/oleobjectcollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [ToList](../../aspose.tasks/oleobjectcollection/tolist/)() | يحوّل نسخة الفئة `OleObjectCollection` إلى قائمة تحتوي على نسخ من الفئة [`OleObject`](../oleobject/). |

## الأمثلة

يظهر كيفية العمل مع مجموعة من كائنات OLE.

```csharp
IDictionary<string, string> extensions = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

// باستخدام الوصول عبر الفهرس
// List<OleObject> list = project.OleObjects.ToList();
// for (var index = 0; index < list.Count; index++)
// {
// var oleObject = list[index];
// }

// أو يمكن للعدّ أن يتنقل عبر كائنات OLE
foreach (var oleObject in project.OleObjects)
{
    if (string.IsNullOrEmpty(oleObject.FileFormat) || !extensions.ContainsKey(oleObject.FileFormat))
    {
        continue;
    }

    var path = OutDir + "EmbeddedContent_" + extensions[oleObject.FileFormat];
    using (var stream = new FileStream(path, FileMode.Create))
    {
        stream.Write(oleObject.Content, 0, oleObject.Content.Length);
    }
}
```

### انظر أيضًا

* class [OleObject](../oleobject/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


