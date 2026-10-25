---
title: "Klasse PrimaveraXerReader"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.PrimaveraXerReader klasse. Vertegenwoordigt een lezer om project‑UID's uit een Primavera XER‑bestand te lezen."
type: docs
weight: 1390
url: /nl/net/aspose.tasks/primaveraxerreader/
---
## PrimaveraXerReader class

Stelt een lezer voor om Project‑UID's uit een Primavera XER‑bestand te lezen

```csharp
public sealed class PrimaveraXerReader : PrimaveraBaseReader
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PrimaveraXerReader](primaveraxerreader/#constructor)(Stream) | Initialiseert een nieuw exemplaar van de `PrimaveraXerReader` klasse. |
| [PrimaveraXerReader](primaveraxerreader/#constructor_1)(string) | Initialiseert een nieuw exemplaar van de `PrimaveraXerReader` klasse. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Retourneer een lijst met de korte informatieobjecten van het project. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Retourneer een lijst met de unieke identificatoren van de projecten. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | Laadt het project met de opgegeven unieke identificator. |

## Voorbeelden

Toont hoe de informatie van korte projecten uit een Primavera XER‑bestand kan worden onderzocht.

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### Zie ook

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


