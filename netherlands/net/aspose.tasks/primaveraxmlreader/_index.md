---
title: "Klasse PrimaveraXmlReader"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.PrimaveraXmlReader klasse. Vertegenwoordigt een lezer die het mogelijk maakt Project‑UID's op te halen uit een Primavera XML‑bestand"
type: docs
weight: 1400
url: /nl/net/aspose.tasks/primaveraxmlreader/
---
## PrimaveraXmlReader class

Stelt een lezer voor die het mogelijk maakt Project‑UID's op te halen uit een Primavera‑Xml‑bestand.

```csharp
public class PrimaveraXmlReader : PrimaveraBaseReader
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor)(Stream) | Initialiseert een nieuw exemplaar van de `PrimaveraXmlReader` klasse. |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor_1)(string) | Initialiseert een nieuw exemplaar van de `PrimaveraXmlReader` klasse. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Retourneer een lijst met de korte informatieobjecten van het project. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Retourneer een lijst met de unieke identificatoren van de projecten. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | Laadt het project met de opgegeven unieke identificator. |

## Voorbeelden

Toont hoe korte projectinformatie te onderzoeken uit een Primavera XML‑bestand.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### Zie ook

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


