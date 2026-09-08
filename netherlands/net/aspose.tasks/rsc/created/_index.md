---
title: "Rsc.Created"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De datum en tijd waarop een resource aan het project is toegevoegd."
type: docs
weight: 260
url: /nl/net/aspose.tasks/rsc/created/
---
## Rsc.Created field

De datum en tijd waarop een resource aan het project is toegevoegd.

```csharp
public static readonly Key<DateTime, RscKey> Created;
```

## Voorbeelden

Toont hoe u de eigenschap Rsc.Created kunt lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + resource.Get(Rsc.Created));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


