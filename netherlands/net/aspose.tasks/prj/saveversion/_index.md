---
title: "Prj.SaveVersion"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. De versie van Microsoft Office Project waarin een projectbestand is opgeslagen"
type: docs
weight: 620
url: /nl/net/aspose.tasks/prj/saveversion/
---
## Prj.SaveVersion field

De versie van Microsoft Office Project waarin een projectbestand is opgeslagen.

```csharp
public static readonly Key<int, PrjKey> SaveVersion;
```

## Voorbeelden

Toont hoe de opslagversie en opslagdatum van een project te controleren.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// Projectversie weergeven
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


