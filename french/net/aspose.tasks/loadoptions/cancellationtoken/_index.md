---
title: "LoadOptions.CancellationToken"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété LoadOptions. Obtient ou définit un jeton qui peut être utilisé pour annuler une opération de chargement de projet."
type: docs
weight: 20
url: /fr/net/aspose.tasks/loadoptions/cancellationtoken/
---
## LoadOptions.CancellationToken property

Obtient ou définit un jeton qui peut être utilisé pour annuler une opération de chargement de projet.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Exemples

Montre comment transmettre CancellationToken pour annuler une opération de chargement de projet de longue durée.

```csharp
var loadOptions = new LoadOptions();

CancellationTokenSource cts = new CancellationTokenSource();
loadOptions.CancellationToken = cts.Token;

// cts peut être transmis à un autre thread où la méthode cts.Cancel() peut être appelée pour annuler l'opération de chargement de projet.
// cts.Cancel();
var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
```

### Voir aussi

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


