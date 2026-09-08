---
title: "SaveTemplateOptions.RemoveFixedCosts"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SaveTemplateOptions-eigenschap. Haalt een waarde op of stelt deze in die aangeeft of alle vaste kosten uit een projectsjabloon moeten worden verwijderd"
type: docs
weight: 40
url: /nl/net/aspose.tasks.saving/savetemplateoptions/removefixedcosts/
---
## SaveTemplateOptions.RemoveFixedCosts property

Haalt of stelt een waarde in die aangeeft of alle vaste kosten uit een projectsjabloon moeten worden verwijderd.

```csharp
public bool RemoveFixedCosts { get; set; }
```

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

* class [SaveTemplateOptions](../)
* namespace [Aspose.Tasks.Saving](../../savetemplateoptions/)
* assembly [Aspose.Tasks](../../../)


