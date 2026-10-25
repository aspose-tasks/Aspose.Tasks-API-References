---
title: "Klasse OleObjectCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.OleObjectCollection-klasse. Vertegenwoordigt een collectie die de instanties van de OleObject-klasse bevat"
type: docs
weight: 1130
url: /nl/net/aspose.tasks/oleobjectcollection/
---
## OleObjectCollection class

Vertegenwoordigt een collectie die de instanties van de [`OleObject`](../oleobject/) klasse bevat.

```csharp
public sealed class OleObjectCollection : IList<OleObject>
```

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Clear](../../aspose.tasks/oleobjectcollection/clear/)() | Leegt de collectie. Om deze wijzigingen te behouden moet project.Save worden aangeroepen met new MPPSaveOptions { WriteViewData = true; } |
| [GetEnumerator](../../aspose.tasks/oleobjectcollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [ToList](../../aspose.tasks/oleobjectcollection/tolist/)() | Converteert de instantie van de `OleObjectCollection`-klasse naar een lijst die de instanties van de [`OleObject`](../oleobject/) klasse bevat. |

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

* class [OleObject](../oleobject/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


