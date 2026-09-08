---
title: "Klasse PrimaveraDbReader"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.PrimaveraDbReader-klasse. Vertegenwoordigt een lezer om projectinformatie uit Primavera DB te lezen"
type: docs
weight: 1350
url: /nl/net/aspose.tasks/primaveradbreader/
---
## PrimaveraDbReader class

Stelt een lezer voor om projectinformatie uit een Primavera‑DB te lezen

```csharp
public sealed class PrimaveraDbReader : PrimaveraBaseReader
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PrimaveraDbReader](primaveradbreader/)(PrimaveraDbSettings) | Initialiseert een nieuw exemplaar van de [`PrimaveraXerReader`](../primaveraxerreader/) klasse. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Retourneer een lijst met de korte informatieobjecten van het project. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Retourneer een lijst met de unieke identificatoren van de projecten. |
| override [LoadProject](../../aspose.tasks/primaveradbreader/loadproject/)(int) | Laadt het project met de opgegeven unieke identificator. |

## Voorbeelden

Toont hoe je beknopte informatie over projecten uit een Primavera-database kunt ophalen.

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### Zie ook

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


