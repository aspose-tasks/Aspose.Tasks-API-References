---
title: "Classe CopyToOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.CopyToOptions. Consente di specificare opzioni aggiuntive durante la copia dei dati del progetto"
type: docs
weight: 340
url: /it/net/aspose.tasks/copytooptions/
---
## CopyToOptions class

Consente di specificare opzioni aggiuntive durante la copia dei dati del progetto.

```csharp
public class CopyToOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [CopyToOptions](copytooptions/)() | Inizializza una nuova istanza della classe `CopyToOptions`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CopyViewData](../../aspose.tasks/copytooptions/copyviewdata/) { get; set; } | Ottiene o imposta un valore che indica se copiare i dati della vista durante la copia dei dati del progetto. Il valore predefinito è true. |

## Esempi

Mostra come utilizzare le opzioni di copia del progetto.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// ignora la copia dei dati della vista durante la copia dei dati comuni del progetto.
var copyToOptions = new CopyToOptions();
copyToOptions.CopyViewData = false;
project.CopyTo(mppProject, copyToOptions);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


