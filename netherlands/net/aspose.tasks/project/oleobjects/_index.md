---
title: "Project.OleObjects"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Projecteigenschap. Haalt een collectie op die de instanties van de OleObject‑klasse bevat die gekoppeld of ingebed zijn in dit projectbestand. Alleen beschikbaar voor mpp‑bestandsformaat. Deze collectie is alleen-lezen, behalve voor de Clear‑bewerking."
type: docs
weight: 700
url: /nl/net/aspose.tasks/project/oleobjects/
---
## Project.OleObjects property

Haalt een collectie op die de instanties van de [`OleObject`](../../oleobject/)‑klasse bevat die gekoppeld of ingebed zijn in dit projectbestand. Alleen beschikbaar voor mpp‑bestandsformaat. Deze collectie is alleen-lezen, behalve voor de 'Clear'‑bewerking.

```csharp
public OleObjectCollection OleObjects { get; }
```

## Voorbeelden

Toont hoe ingebedde OLE‑objecten te extraheren.

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

### Zie ook

* class [OleObjectCollection](../../oleobjectcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


