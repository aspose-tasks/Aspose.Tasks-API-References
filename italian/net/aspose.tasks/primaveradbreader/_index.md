---
title: "Classe PrimaveraDbReader"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.PrimaveraDbReader. Rappresenta un lettore per leggere le informazioni del progetto dal DB Primavera."
type: docs
weight: 1350
url: /it/net/aspose.tasks/primaveradbreader/
---
## PrimaveraDbReader class

Rappresenta un lettore per leggere le informazioni del progetto dal DB Primavera

```csharp
public sealed class PrimaveraDbReader : PrimaveraBaseReader
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PrimaveraDbReader](primaveradbreader/)(PrimaveraDbSettings) | Inizializza una nuova istanza della classe [`PrimaveraXerReader`](../primaveraxerreader/). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Restituisce un elenco degli oggetti di informazioni brevi del progetto. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Restituisci un elenco degli identificatori univoci dei progetti. |
| override [LoadProject](../../aspose.tasks/primaveradbreader/loadproject/)(int) | Carica il progetto con l'identificatore univoco specificato. |

## Esempi

Mostra come ottenere informazioni brevi sui progetti da un database Primavera.

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### Vedi anche

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


