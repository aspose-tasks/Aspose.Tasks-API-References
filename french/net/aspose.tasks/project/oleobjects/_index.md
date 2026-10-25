---
title: "Project.OleObjects"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Project property. Obtient une collection contenant les instances de la classe OleObject qui sont liées ou incorporées à ce fichier de projet. Disponible uniquement pour le format de fichier mpp. Cette collection est en lecture seule sauf pour l'opération Clear."
type: docs
weight: 700
url: /fr/net/aspose.tasks/project/oleobjects/
---
## Project.OleObjects property

Obtient une collection contenant les instances de la classe [`OleObject`](../../oleobject/) qui sont liées ou incorporées à ce fichier de projet. Disponible uniquement pour le format de fichier mpp. Cette collection est en lecture seule sauf pour l'opération 'Clear'.

```csharp
public OleObjectCollection OleObjects { get; }
```

## Exemples

Montre comment extraire des objets OLE incorporés.

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

### Voir aussi

* class [OleObjectCollection](../../oleobjectcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


