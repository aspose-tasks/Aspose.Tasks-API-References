---
title: "PrimaveraXmlReader.PrimaveraXmlReader"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore PrimaveraXmlReader. Inizializza una nuova istanza della classe PrimaveraXmlReader"
type: docs
weight: 10
url: /it/net/aspose.tasks/primaveraxmlreader/primaveraxmlreader/
---
## PrimaveraXmlReader(string) {#constructor_1}

Inizializza una nuova istanza della classe [`PrimaveraXmlReader`](../).

```csharp
public PrimaveraXmlReader(string templatePath)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| templatePath | Stringa | Percorso del modello in cui è situato il progetto Primavera Xml o i progetti |

## Esempi

Mostra come esaminare le informazioni di progetti brevi da un file XML Primavera.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### Vedi anche

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXmlReader(Stream) {#constructor}

Inizializza una nuova istanza della classe [`PrimaveraXmlReader`](../).

```csharp
public PrimaveraXmlReader(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | Flusso | Flusso contenente contenuto Primavera Xml. |

## Esempi

Mostra come importare un progetto da un flusso Primavera XML.

```csharp
using (var stream = new FileStream(DataDir + "primavera.xml", FileMode.Open))
{
    var reader = new PrimaveraXmlReader(stream);
    List<int> projectUids = reader.GetProjectUids();
    foreach (var projectUid in projectUids)
    {
        Console.WriteLine("Project UID: " + projectUid);
    }
}
```

### Vedi anche

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)


