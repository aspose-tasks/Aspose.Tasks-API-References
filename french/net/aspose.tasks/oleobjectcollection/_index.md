---
title: "Classe OleObjectCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.OleObjectCollection. Représente une collection contenant les instances de la classe OleObject"
type: docs
weight: 1130
url: /fr/net/aspose.tasks/oleobjectcollection/
---
## OleObjectCollection class

Représente une collection contenant les instances de la classe [`OleObject`](../oleobject/).

```csharp
public sealed class OleObjectCollection : IList<OleObject>
```

## Méthodes

| Nom | Description |
| --- | --- |
| [Clear](../../aspose.tasks/oleobjectcollection/clear/)() | Efface la collection. Afin de persister ces modifications, project.Save doit être appelé avec new MPPSaveOptions { WriteViewData = true; } |
| [GetEnumerator](../../aspose.tasks/oleobjectcollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [ToList](../../aspose.tasks/oleobjectcollection/tolist/)() | Convertit l'instance de la classe `OleObjectCollection` en une liste contenant les instances de la classe [`OleObject`](../oleobject/). |

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

* class [OleObject](../oleobject/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


