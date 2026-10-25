---
title: "Project.RemoveInvalidResourceAssignments"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project-methode. Elimineert ongeldige resource‑toewijzingen uit de lijst met resource‑toewijzingen van het project"
type: docs
weight: 1170
url: /nl/net/aspose.tasks/project/removeinvalidresourceassignments/
---
## Project.RemoveInvalidResourceAssignments method

Verwijdert ongeldige resource-toewijzingen uit de lijst met projectresource-toewijzingen.

```csharp
public void RemoveInvalidResourceAssignments()
```

## Opmerkingen

MS Project maakt een lege resource‑toewijzing aan voor elke taak. Roep de methode aan om ze te verwijderen.

## Voorbeelden

Toont hoe ongeldige toewijzingen te verwijderen.

```csharp
var project = new Project(DataDir + "InvalidResourceAssignments.mpp");
var invalid = 0;

// ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
foreach (var ra in project.ResourceAssignments)
{
    if (ra.Get(Asn.Resource) == null)
    {
        invalid++;
    }
}

Console.WriteLine("Count of invalid assignments (before): " + invalid);

// verwijder ongeldige toewijzingen
project.RemoveInvalidResourceAssignments();

Console.WriteLine("Count of invalid assignments (after): " + invalid);
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


