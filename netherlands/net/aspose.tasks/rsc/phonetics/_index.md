---
title: "Rsc.Phonetics"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De fonetische spelling van de resource‑naam. Alleen voor gebruik met Japans."
type: docs
weight: 560
url: /nl/net/aspose.tasks/rsc/phonetics/
---
## Rsc.Phonetics field

De fonetische spelling van de resource-naam. Alleen voor gebruik met Japans.

```csharp
public static readonly Key<string, RscKey> Phonetics;
```

## Voorbeelden

Toont hoe u de eigenschap Rsc.Phonetics kunt lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Phonetics, "Phonetics");

Console.WriteLine("Phonetics: " + resource.Get(Rsc.Phonetics));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


