---
title: Project.OleObjects
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets a collection containing the instances of the OleObject class which are linked or embedded to this project file. Available for mpp file format only. This collection is readonly except for Clear operation
type: docs
weight: 690
url: /net/aspose.tasks/project/oleobjects/
---
## Project.OleObjects property

Gets a collection containing the instances of the [`OleObject`](../../oleobject/) class which are linked or embedded to this project file. Available for mpp file format only. This collection is read-only except for 'Clear' operation.

```csharp
public OleObjectCollection OleObjects { get; }
```

## Examples

Shows how to extract an embedded OLE objects.

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

### See Also

* class [OleObjectCollection](../../oleobjectcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


