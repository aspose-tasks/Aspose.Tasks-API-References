---
title: "Project.GetWork"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Projectmethode. Haalt Duration-object op met de opgegeven Double-waarde en standaard werkformaat"
type: docs
weight: 1130
url: /nl/net/aspose.tasks/project/getwork/
---
## Project.GetWork method

Haalt [`Duration`](../../duration/) object op met de opgegeven Double-waarde en standaard werkformaat.

```csharp
public Duration GetWork(double val)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | Double | opgegeven double-waarde. |

### Retourwaarde

Duration-object.

## Opmerkingen

Deze methode moet zorgvuldig worden gebruikt omdat deze verschillende duurwaarden retourneert, afhankelijk van de instelling van Project.WorkFormat. Bijvoorbeeld, GetWork(1.0) retourneert 1 uur wanneer Project.WorkFormat TimeUnitType.Hour is of 1 dag als Project.WorkFormat TimeUnitType.Day is.

## Voorbeelden

Toont hoe een werk op te halen met het standaard werkformaat.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// maak een werkwaarde met het standaard werkformaat van het project
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### Zie ook

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


