---
title: "OleObjectCollection.ToList"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة OleObjectCollection. تُحوّل نسخة من فئة OleObjectCollection إلى قائمة تحتوي على نسخ من فئة OleObject"
type: docs
weight: 30
url: /ar/net/aspose.tasks/oleobjectcollection/tolist/
---
## OleObjectCollection.ToList method

يُحوّل نسخة من الفئة [`OleObjectCollection`](../) إلى قائمة تحتوي على نسخ من الفئة [`OleObject`](../../oleobject/).

```csharp
public List<OleObject> ToList()
```

### قيمة الإرجاع

تم تحويل نسخة من الفئة [`OleObjectCollection`](../) إلى قائمة تحتوي على نسخ من الفئة [`OleObject`](../../oleobject/).

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

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


