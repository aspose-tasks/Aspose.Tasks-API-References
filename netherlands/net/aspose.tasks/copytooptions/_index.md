---
title: "Klasse CopyToOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.CopyToOptions klasse. Stelt u in staat extra opties op te geven bij het kopiëren van projectgegevens"
type: docs
weight: 340
url: /nl/net/aspose.tasks/copytooptions/
---
## CopyToOptions class

Staat toe om extra opties op te geven bij het kopiëren van projectgegevens.

```csharp
public class CopyToOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [CopyToOptions](copytooptions/)() | Initialiseert een nieuw exemplaar van de `CopyToOptions` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CopyViewData](../../aspose.tasks/copytooptions/copyviewdata/) { get; set; } | Haalt of stelt een waarde in die aangeeft of weergavegegevens moeten worden gekopieerd tijdens het kopiëren van projectgegevens. Standaardwaarde is true. |

## Voorbeelden

Toont hoe projectkopieeropties te gebruiken.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// sla kopiëren van weergavegegevens over tijdens het kopiëren van algemene projectgegevens.
var copyToOptions = new CopyToOptions();
copyToOptions.CopyViewData = false;
project.CopyTo(mppProject, copyToOptions);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


