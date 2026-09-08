---
title: "Klasse PrimaveraReadOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.PrimaveraReadOptions-klasse. Stelt u in staat extra opties op te geven bij het lezen van Primavera Xml- of Primavera Xer-bestanden"
type: docs
weight: 1370
url: /nl/net/aspose.tasks/primaverareadoptions/
---
## PrimaveraReadOptions class

Staat toe om extra opties te specificeren bij het lezen van Primavera‑Xml‑ of Primavera‑Xer‑bestanden.

```csharp
public class PrimaveraReadOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PrimaveraReadOptions](primaverareadoptions/)() | Initialiseert een nieuw exemplaar van de `PrimaveraReadOptions`-klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [PreserveUids](../../aspose.tasks/primaverareadoptions/preserveuids/) { get; set; } | Haalt of stelt een vlag in die aangeeft of originele unieke identifiers van entiteiten behouden moeten blijven. |
| [ProjectUid](../../aspose.tasks/primaverareadoptions/projectuid/) { get; set; } | Haalt of stelt de UID van een project in die gelezen moet worden uit een bestand met meerdere projecten. |
| [ReadBaselineProjects](../../aspose.tasks/primaverareadoptions/readbaselineprojects/) { get; set; } | Haalt of stelt een vlag in die aangeeft of baseline-projecten geladen moeten worden. De standaardwaarde is true. |
| [UndefinedConstraintHandlingBehavior](../../aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/) { get; set; } | Specificeert het gedrag dat wordt gebruikt om taken met ongedefinieerde beperkingen, gelezen uit XER-indeling, te verwerken. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


