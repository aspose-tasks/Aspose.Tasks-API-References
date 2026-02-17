---
title: Class OleObjectCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.OleObjectCollection class. Represents a collection containing the instances of the OleObject class
type: docs
weight: 1120
url: /net/aspose.tasks/oleobjectcollection/
---
## OleObjectCollection class

Represents a collection containing the instances of the [`OleObject`](../oleobject/) class.

```csharp
public sealed class OleObjectCollection : IList<OleObject>
```

## Methods

| Name | Description |
| --- | --- |
| [Clear](../../aspose.tasks/oleobjectcollection/clear/)() | Clears the collection. In order to persist these changes project.Save should be called with new MPPSaveOptions { WriteViewData = true; } |
| [GetEnumerator](../../aspose.tasks/oleobjectcollection/getenumerator/)() | Returns an enumerator for this collection. |
| [ToList](../../aspose.tasks/oleobjectcollection/tolist/)() | Converts the instance of the `OleObjectCollection` class to a list containing the instances of the [`OleObject`](../oleobject/) class. |

## Examples

Shows how to work with collection of OLE objects.

```csharp
IDictionary<string, string> extensions = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

// by using index access
// List<OleObject> list = project.OleObjects.ToList();
// for (var index = 0; index < list.Count; index++)
// {
// var oleObject = list[index];
// }

// or enumeration one can iterate over OLE objects
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

### See Also

* class [OleObject](../oleobject/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


