---
title: "OleObjectCollection.ToList"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode OleObjectCollection. Convertit l'instance de la classe OleObjectCollection en une liste contenant les instances de la classe OleObject"
type: docs
weight: 30
url: /fr/net/aspose.tasks/oleobjectcollection/tolist/
---
## OleObjectCollection.ToList method

Convertit l'instance de la classe [`OleObjectCollection`](../) en une liste contenant les instances de la classe [`OleObject`](../../oleobject/).

```csharp
public List<OleObject> ToList()
```

### Valeur de retour

Converti en liste l'instance de la classe [`OleObjectCollection`](../) contenant les instances de la classe [`OleObject`](../../oleobject/).

## Exemples

Montre comment travailler avec une collection d'objets OLE.

```csharp
IDictionary<string, string> extensions = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

// en utilisant l'accès par indice
// List<OleObject> list = project.OleObjects.ToList();
// for (var index = 0; index < list.Count; index++)
// {
// var oleObject = list[index];
// }

// ou énumération, on peut parcourir les objets OLE
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

### Voir aussi

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


