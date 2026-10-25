---
title: "Project.OleObjects"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà del progetto. Ottiene una collezione contenente le istanze della classe OleObject che sono collegate o incorporate in questo file di progetto. Disponibile solo per il formato file mpp. Questa collezione è di sola lettura eccetto l'operazione Clear."
type: docs
weight: 700
url: /it/net/aspose.tasks/project/oleobjects/
---
## Project.OleObjects property

Ottiene una collezione contenente le istanze della classe [`OleObject`](../../oleobject/) che sono collegate o incorporate in questo file di progetto. Disponibile solo per il formato file mpp. Questa collezione è di sola lettura eccetto l'operazione 'Clear'.

```csharp
public OleObjectCollection OleObjects { get; }
```

## Esempi

Mostra come estrarre oggetti OLE incorporati.

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

### Vedi anche

* class [OleObjectCollection](../../oleobjectcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


