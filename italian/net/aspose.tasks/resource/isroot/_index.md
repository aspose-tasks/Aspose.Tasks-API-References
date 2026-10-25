---
title: "Resource.IsRoot"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Resource. Ottiene il flag che indica se la risorsa è una risorsa radice. La risorsa radice è una risorsa speciale destinata a supportare gli aspetti interni dei formati MS Projects e non è destinata a essere utilizzata direttamente dal codice degli utenti"
type: docs
weight: 470
url: /it/net/aspose.tasks/resource/isroot/
---
## Resource.IsRoot property

Ottiene il flag che indica se la risorsa è una risorsa radice. La risorsa radice è una risorsa speciale destinata a supportare gli internals dei formati di MS Project e non è destinata a essere utilizzata direttamente dal codice dell'utente.

```csharp
public virtual bool IsRoot { get; }
```

## Esempi

Mostra come utilizzare la proprietà IsRoot per saltare la risorsa radice.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

foreach (var resource in project.Resources)
{
    if (resource.IsRoot)
    {
        continue;
    }

    Console.WriteLine(resource.Get(Rsc.Name));
}
```

### Vedi anche

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


