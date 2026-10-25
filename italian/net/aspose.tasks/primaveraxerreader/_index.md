---
title: "Classe PrimaveraXerReader"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.PrimaveraXerReader. Rappresenta un lettore per leggere gli UID del progetto da un file Primavera XER"
type: docs
weight: 1390
url: /it/net/aspose.tasks/primaveraxerreader/
---
## PrimaveraXerReader class

Rappresenta un lettore per leggere gli UID del progetto da un file Primavera XER

```csharp
public sealed class PrimaveraXerReader : PrimaveraBaseReader
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PrimaveraXerReader](primaveraxerreader/#constructor)(Stream) | Inizializza una nuova istanza della classe `PrimaveraXerReader`. |
| [PrimaveraXerReader](primaveraxerreader/#constructor_1)(string) | Inizializza una nuova istanza della classe `PrimaveraXerReader`. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Restituisce un elenco degli oggetti di informazioni brevi del progetto. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Restituisci un elenco degli identificatori univoci dei progetti. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | Carica il progetto con l'identificatore univoco specificato. |

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

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


