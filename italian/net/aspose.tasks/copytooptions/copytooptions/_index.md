---
title: "CopyToOptions.CopyToOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore di CopyToOptions. Inizializza una nuova istanza della classe CopyToOptions"
type: docs
weight: 10
url: /it/net/aspose.tasks/copytooptions/copytooptions/
---
## CopyToOptions constructor

Inizializza una nuova istanza della classe [`CopyToOptions`](../).

```csharp
public CopyToOptions()
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


