---
title: "Klasse PrimaveraDbReader"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Aspose.Tasks.PrimaveraDbReader-Klasse. Stellt einen Leser zum Auslesen von Projektinformationen aus der Primavera-DB dar."
type: docs
weight: 1350
url: /de/net/aspose.tasks/primaveradbreader/
---
## PrimaveraDbReader class

Stellt einen Leser zum Auslesen von Projektinformationen aus der Primavera-DB dar.

```csharp
public sealed class PrimaveraDbReader : PrimaveraBaseReader
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PrimaveraDbReader](primaveradbreader/)(PrimaveraDbSettings) | Initialisiert eine neue Instanz der Klasse [`PrimaveraXerReader`](../primaveraxerreader/) . |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Gibt eine Liste der Kurzinfo-Objekte des Projekts zurück. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Gibt eine Liste der eindeutigen Bezeichner der Projekte zurück. |
| override [LoadProject](../../aspose.tasks/primaveradbreader/loadproject/)(int) | Lädt das Projekt mit dem angegebenen eindeutigen Bezeichner. |

## Beispiele

Zeigt, wie man kurze Informationen zu Projekten aus einer Primavera-Datenbank erhält.

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

### Siehe auch

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


