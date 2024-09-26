---
title: OleObjectCollection.GetEnumerator
second_title: Aspose.Tasks for .NET API Reference
description: OleObjectCollection method. Returns an enumerator for this collection
type: docs
weight: 20
url: /net/aspose.tasks/oleobjectcollection/getenumerator/
---
## OleObjectCollection.GetEnumerator method

Returns an enumerator for this collection.

```csharp
public IEnumerator<OleObject> GetEnumerator()
```

### Return Value

an enumerator for this collection.

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

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


