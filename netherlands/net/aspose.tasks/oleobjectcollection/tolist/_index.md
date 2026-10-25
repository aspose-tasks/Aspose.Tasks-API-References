---
title: "OleObjectCollection.ToList"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "OleObjectCollection-methode. Converteert de instantie van de OleObjectCollection-klasse naar een lijst met de instanties van de OleObject-klasse"
type: docs
weight: 30
url: /nl/net/aspose.tasks/oleobjectcollection/tolist/
---
## OleObjectCollection.ToList method

Converteert de instantie van de [`OleObjectCollection`](../) klasse naar een lijst met de instanties van de [`OleObject`](../../oleobject/) klasse.

```csharp
public List<OleObject> ToList()
```

### Retourwaarde

Geconverteerd naar een lijst de instantie van de [`OleObjectCollection`](../) klasse die de instanties van de [`OleObject`](../../oleobject/) klasse bevat.

## Voorbeelden

Toont hoe je met een collectie van OLE-objecten werkt.

```csharp
IDictionary<string, string> extensions = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

// door indextoegang te gebruiken
// List<OleObject> list = project.OleObjects.ToList();
// for (var index = 0; index < list.Count; index++)
// {
// var oleObject = list[index];
// }

// of enumeratie kan men itereren over OLE-objecten
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

### Zie ook

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


