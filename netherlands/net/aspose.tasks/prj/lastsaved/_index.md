---
title: "Prj.LastSaved"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj veld. De datum waarop een project voor het laatst is opgeslagen. Opgeslagen in UTC-formaat in mpp-bestanden. Type DateTime"
type: docs
weight: 440
url: /nl/net/aspose.tasks/prj/lastsaved/
---
## Prj.LastSaved field

De datum waarop een project voor het laatst is opgeslagen. Opgeslagen in UTC-formaat in mpp-bestanden. Type DateTime.

```csharp
public static readonly Key<DateTime, PrjKey> LastSaved;
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


