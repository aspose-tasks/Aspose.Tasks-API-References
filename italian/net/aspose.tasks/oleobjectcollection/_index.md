---
title: "Classe OleObjectCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.OleObjectCollection. Rappresenta una raccolta contenente le istanze della classe OleObject"
type: docs
weight: 1130
url: /it/net/aspose.tasks/oleobjectcollection/
---
## OleObjectCollection class

Rappresenta una raccolta contenente le istanze della classe [`OleObject`](../oleobject/).

```csharp
public sealed class OleObjectCollection : IList<OleObject>
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Clear](../../aspose.tasks/oleobjectcollection/clear/)() | Cancella la raccolta. Per rendere persistenti queste modifiche, dovrebbe essere chiamato project.Save con new MPPSaveOptions { WriteViewData = true; } |
| [GetEnumerator](../../aspose.tasks/oleobjectcollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [ToList](../../aspose.tasks/oleobjectcollection/tolist/)() | Converte l'istanza della classe `OleObjectCollection` in un elenco contenente le istanze della classe [`OleObject`](../oleobject/). |

## Esempi

Mostra come lavorare con una raccolta di oggetti OLE.

```csharp
IDictionary<string, string> extensions = new Dictionary<string, string>
{
    { "RTF", "_rtfFile_out.rtf" },
    { "MSWordDoc", "_wordFile_out.docx" },
    { "ExcelML12", "_excelFile_out.xlsx" }
};

var project = new Project(DataDir + "Embedded.mpp");

// utilizzando l'accesso per indice
// List<OleObject> list = project.OleObjects.ToList();
// for (var index = 0; index < list.Count; index++)
// {
// var oleObject = list[index];
// }

// oppure l'enumerazione consente di iterare sugli oggetti OLE
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

### Vedi anche

* class [OleObject](../oleobject/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


