---
title: "Class SaveTemplateOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Saving.SaveTemplateOptions class. Stelt u in staat extra opties op te geven bij het opslaan van een project als sjabloon"
type: docs
weight: 2200
url: /nl/net/aspose.tasks.saving/savetemplateoptions/
---
## SaveTemplateOptions class

Staat toe extra opties op te geven bij het opslaan van een project als sjabloon.

```csharp
public class SaveTemplateOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [SaveTemplateOptions](savetemplateoptions/)() | De standaardconstructor. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [RemoveActualValues](../../aspose.tasks.saving/savetemplateoptions/removeactualvalues/) { get; set; } | Haalt of stelt een waarde in die aangeeft of alle feitelijke waarden uit een projectsjabloon moeten worden verwijderd. |
| [RemoveBaselineValues](../../aspose.tasks.saving/savetemplateoptions/removebaselinevalues/) { get; set; } | Haalt of stelt een waarde in die aangeeft of alle basislijnwaarden uit een projectsjabloon moeten worden verwijderd. |
| [RemoveFixedCosts](../../aspose.tasks.saving/savetemplateoptions/removefixedcosts/) { get; set; } | Haalt of stelt een waarde in die aangeeft of alle vaste kosten uit een projectsjabloon moeten worden verwijderd. |
| [RemoveResourceRates](../../aspose.tasks.saving/savetemplateoptions/removeresourcerates/) { get; set; } | Haalt of stelt een waarde in die aangeeft of resource tarieven uit een projectsjabloon moeten worden verwijderd. |

## Voorbeelden

Toont hoe een project als sjabloon kan worden opgeslagen met behulp van opties.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var projectFileInfo = Project.GetProjectFileInfo(DataDir + "EstimatedMilestoneTasks.mpp");

Console.WriteLine("Project File Format: " + projectFileInfo.ProjectFileFormat);

// maak sjabloon opslaan opties
// en stem de eigenschappen af
var options = new SaveTemplateOptions
{
    // stel een waarde in die aangeeft of alle vaste kosten uit een projectsjabloon moeten worden verwijderd
    RemoveFixedCosts = true,

    // stel een waarde in die aangeeft of alle feitelijke waarden uit een projectsjabloon moeten worden verwijderd
    RemoveActualValues = true,

    // stel een waarde in die aangeeft of resource tarieven uit een projectsjabloon moeten worden verwijderd
    RemoveResourceRates = true,

    // stel een waarde in die aangeeft of alle basislijnwaarden uit een projectsjabloon moeten worden verwijderd
    RemoveBaselineValues = true
};

project.SaveAsTemplate(OutDir + "SaveProjectDataAsTemplate_out.mpt", options);

var templateFileInfo = Project.GetProjectFileInfo(DataDir + "SaveProjectDataAsTemplate_out.mpt");
Console.WriteLine("Project File Format: " + templateFileInfo.ProjectFileFormat);
```

### Zie ook

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


