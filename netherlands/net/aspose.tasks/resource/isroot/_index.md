---
title: "Resource.IsRoot"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Resource-eigenschap. Haalt de vlag op die aangeeft of de resource een root-resource is. Een root-resource is een speciale resource die bedoeld is om de interne werking van MS Projects-formaten te ondersteunen en niet bedoeld is om direct vanuit de code van de gebruiker te worden gebruikt."
type: docs
weight: 470
url: /nl/net/aspose.tasks/resource/isroot/
---
## Resource.IsRoot property

Haalt de vlag op die aangeeft of de resource een rootresource is. Een rootresource is een speciale resource die bedoeld is om de interne werking van de formaten van MS Project te ondersteunen en niet bedoeld is om direct vanuit de code van de gebruiker te worden gebruikt.

```csharp
public virtual bool IsRoot { get; }
```

## Voorbeelden

Toont hoe de IsRoot-eigenschap gebruikt kan worden om root-resources over te slaan.

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

### Zie ook

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


