---
title: "PrimaveraReadOptions.ProjectUid"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PrimaveraReadOptions eigenschap. Haalt of stelt de UID van een project in dat moet worden gelezen uit een bestand met meerdere projecten"
type: docs
weight: 30
url: /nl/net/aspose.tasks/primaverareadoptions/projectuid/
---
## PrimaveraReadOptions.ProjectUid property

Haalt of stelt de UID van een project in die gelezen moet worden uit een bestand met meerdere projecten.

```csharp
public int ProjectUid { get; set; }
```

## Voorbeelden

Toont hoe u een project kunt lezen uit een Primavera XML- of Primavera XER-bestand met meerdere projecten.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// Retourneert project met speciale UID
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### Zie ook

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


