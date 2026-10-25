---
title: "Project.OleObjects"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. يحصل على مجموعة تحتوي على مثيلات فئة OleObject المرتبطة أو المضمنة في ملف المشروع هذا. متاح لتنسيق ملف mpp فقط. هذه المجموعة للقراءة فقط باستثناء عملية Clear."
type: docs
weight: 700
url: /ar/net/aspose.tasks/project/oleobjects/
---
## Project.OleObjects property

يحصل على مجموعة تحتوي على مثيلات فئة [`OleObject`](../../oleobject/) المرتبطة أو المضمنة في ملف المشروع هذا. متاح لتنسيق ملف mpp فقط. هذه المجموعة للقراءة فقط باستثناء عملية 'Clear'.

```csharp
public OleObjectCollection OleObjects { get; }
```

## الأمثلة

يظهر كيفية استخراج كائنات OLE المضمنة.

```csharp
IDictionary<string, string> formatExt = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

foreach (var oleObject in project.OleObjects)
{
    if (string.IsNullOrEmpty(oleObject.FileFormat) || !formatExt.ContainsKey(oleObject.FileFormat))
    {
        continue;
    }

    var path = OutDir + "EmbeddedContent_" + formatExt[oleObject.FileFormat];
    using (var stream = new FileStream(path, FileMode.Create))
    {
        stream.Write(oleObject.Content, 0, oleObject.Content.Length);
    }
}
```

### انظر أيضًا

* class [OleObjectCollection](../../oleobjectcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


