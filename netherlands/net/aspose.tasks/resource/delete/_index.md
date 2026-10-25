---
title: "Resource.Delete"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Resource-methode. Verwijdert een resource en de bijbehorende toewijzingen uit het project"
type: docs
weight: 810
url: /nl/net/aspose.tasks/resource/delete/
---
## Resource.Delete method

Verwijdert een resource en de bijbehorende toewijzingen uit het project.

```csharp
public void Delete()
```

## Voorbeelden

Toont hoe je een resource verwijdert.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource = project.Resources.GetById(1);

Console.WriteLine("Number of resources (before): " + project.Resources.Count);

// verwijder de resource
resource.Delete();

Console.WriteLine("Number of resources (after): " + project.Resources.Count);
```

### Zie ook

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


