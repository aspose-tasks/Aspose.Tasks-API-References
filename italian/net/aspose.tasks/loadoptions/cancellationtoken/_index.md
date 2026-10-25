---
title: "LoadOptions.CancellationToken"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà LoadOptions. Ottiene o imposta un token che può essere usato per annullare un'operazione di caricamento del progetto."
type: docs
weight: 20
url: /it/net/aspose.tasks/loadoptions/cancellationtoken/
---
## LoadOptions.CancellationToken property

Ottiene o imposta un token che può essere usato per annullare un'operazione di caricamento del progetto.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Esempi

Mostra come passare CancellationToken per annullare un'operazione di caricamento del progetto a lungo termine.

```csharp
var loadOptions = new LoadOptions();

CancellationTokenSource cts = new CancellationTokenSource();
loadOptions.CancellationToken = cts.Token;

// cts può essere passato a un altro thread dove il metodo cts.Cancel() può essere chiamato per annullare l'operazione di caricamento del progetto.
// cts.Cancel();
var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
```

### Vedi anche

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


