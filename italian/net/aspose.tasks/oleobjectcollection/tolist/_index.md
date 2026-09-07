---
title: "OleObjectCollection.ToList"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo OleObjectCollection. Converte l'istanza della classe OleObjectCollection in una lista contenente le istanze della classe OleObject"
type: docs
weight: 30
url: /it/net/aspose.tasks/oleobjectcollection/tolist/
---
## OleObjectCollection.ToList method

Converte l'istanza della classe [`OleObjectCollection`](../) in una lista contenente le istanze della classe [`OleObject`](../../oleobject/).

```csharp
public List<OleObject> ToList()
```

### Valore di ritorno

Convertita in lista l'istanza della classe [`OleObjectCollection`](../) contenente le istanze della classe [`OleObject`](../../oleobject/).

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

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


