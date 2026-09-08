---
title: "LoadOptions.CancellationToken"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "LoadOptions-eigenschap. Haalt op of stelt een token in dat kan worden gebruikt om een projectlaadbewerking te annuleren."
type: docs
weight: 20
url: /nl/net/aspose.tasks/loadoptions/cancellationtoken/
---
## LoadOptions.CancellationToken property

Haalt een token op of stelt deze in die kan worden gebruikt om een projectlaadoperatie te annuleren.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Voorbeelden

Toont hoe een CancellationToken kan worden doorgegeven om een langdurige projectlaadbewerking te annuleren.

```csharp
var loadOptions = new LoadOptions();

CancellationTokenSource cts = new CancellationTokenSource();
loadOptions.CancellationToken = cts.Token;

// cts kan worden doorgegeven aan een andere thread waar de methode cts.Cancel() kan worden aangeroepen om de projectlaadbewerking te annuleren.
// cts.Cancel();
var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
```

### Zie ook

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


