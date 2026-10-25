---
title: "PrimaveraXerReader.PrimaveraXerReader"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore di PrimaveraXerReader. Inizializza una nuova istanza della classe PrimaveraXerReader"
type: docs
weight: 10
url: /it/net/aspose.tasks/primaveraxerreader/primaveraxerreader/
---
## PrimaveraXerReader(string) {#constructor_1}

Inizializza una nuova istanza della classe [`PrimaveraXerReader`](../).

```csharp
public PrimaveraXerReader(string xerFilePath)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| xerFilePath | Stringa | Percorso al file .xer in cui è situato il progetto o i progetti Primavera. |

## Esempi

Mostra come esaminare le informazioni dei progetti brevi da un file Primavera XER.

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### Vedi anche

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXerReader(Stream) {#constructor}

Inizializza una nuova istanza della classe [`PrimaveraXerReader`](../).

```csharp
public PrimaveraXerReader(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | Flusso | Stream con contenuto XER di Primavera. |

### Vedi anche

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)


