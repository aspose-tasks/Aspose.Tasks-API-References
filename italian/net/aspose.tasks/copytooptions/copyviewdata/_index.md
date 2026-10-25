---
title: "CopyToOptions.CopyViewData"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà CopyToOptions. Ottiene o imposta un valore che indica se copiare i dati di visualizzazione durante la copia dei dati del progetto. Il valore predefinito è true"
type: docs
weight: 20
url: /it/net/aspose.tasks/copytooptions/copyviewdata/
---
## CopyToOptions.CopyViewData property

Ottiene o imposta un valore che indica se copiare i dati della vista durante la copia dei dati del progetto. Il valore predefinito è true.

```csharp
public bool CopyViewData { get; set; }
```

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

* class [CopyToOptions](../)
* namespace [Aspose.Tasks](../../copytooptions/)
* assembly [Aspose.Tasks](../../../)


