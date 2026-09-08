---
title: "Klasse ProjectFileInfo."
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ProjectFileInfo-klasse. Het klasse‑exemplaar bevat informatie over het projectbestandsformaat en de versie van Microsoft Project waarin het bestand is gemaakt."
type: docs
weight: 1460
url: /nl/net/aspose.tasks/projectfileinfo/
---
## ProjectFileInfo class

De klasse‑instantie bevat informatie over het project‑bestandformaat en de versie van Microsoft Project waarin het bestand is gemaakt.

```csharp
public sealed class ProjectFileInfo : IEquatable<ProjectFileInfo>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CanRead](../../aspose.tasks/projectfileinfo/canread/) { get; } | Haalt een waarde op die aangeeft of Aspose.Tasks het projectbestand kan verwerken. |
| [IsPasswordProtected](../../aspose.tasks/projectfileinfo/ispasswordprotected/) { get; } | Haalt een waarde op die aangeeft of een project met een wachtwoord is beveiligd. |
| [ProjectApplicationInfo](../../aspose.tasks/projectfileinfo/projectapplicationinfo/) { get; } | Haalt de toepassingsinformatie van het projectbestand op. |
| [ProjectFileFormat](../../aspose.tasks/projectfileinfo/projectfileformat/) { get; } | Haalt het projectbestandsformaat op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [Equals](../../aspose.tasks/projectfileinfo/equals/#equals_1)(object) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [Equals](../../aspose.tasks/projectfileinfo/equals/#equals)(ProjectFileInfo) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| override [GetHashCode](../../aspose.tasks/projectfileinfo/gethashcode/)() | Retourneert een hashcode‑waarde voor het exemplaar van de `ProjectFileInfo`‑klasse. |

## Opmerkingen

Gebruik de CanRead‑eigenschap om te definiëren dat de bibliotheek het projectbestand kan verwerken.

## Voorbeelden

Toont hoe je projectbestandsinformatie kunt lezen.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


