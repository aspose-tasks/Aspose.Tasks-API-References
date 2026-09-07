---
title: "SaveTemplateOptions.RemoveFixedCosts"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "SaveTemplateOptions proprietà. Ottiene o imposta un valore che indica se tutti i costi fissi da un modello di progetto devono essere rimossi"
type: docs
weight: 40
url: /it/net/aspose.tasks.saving/savetemplateoptions/removefixedcosts/
---
## SaveTemplateOptions.RemoveFixedCosts property

Ottiene o imposta un valore che indica se tutti i costi fissi da un modello di progetto devono essere rimossi.

```csharp
public bool RemoveFixedCosts { get; set; }
```

## Esempi

Mostra come salvare un progetto come modello utilizzando le opzioni.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var projectFileInfo = Project.GetProjectFileInfo(DataDir + "EstimatedMilestoneTasks.mpp");

Console.WriteLine("Project File Format: " + projectFileInfo.ProjectFileFormat);

// crea opzioni di salvataggio del modello
// e regola le sue proprietà
var options = new SaveTemplateOptions
{
    // imposta un valore che indica se tutti i costi fissi da un modello di progetto devono essere rimossi
    RemoveFixedCosts = true,

    // imposta un valore che indica se tutti i valori effettivi da un modello di progetto devono essere rimossi
    RemoveActualValues = true,

    // imposta un valore che indica se le tariffe delle risorse da un modello di progetto devono essere rimosse
    RemoveResourceRates = true,

    // imposta un valore che indica se tutti i valori di baseline da un modello di progetto devono essere rimossi
    RemoveBaselineValues = true
};

project.SaveAsTemplate(OutDir + "SaveProjectDataAsTemplate_out.mpt", options);

var templateFileInfo = Project.GetProjectFileInfo(DataDir + "SaveProjectDataAsTemplate_out.mpt");
Console.WriteLine("Project File Format: " + templateFileInfo.ProjectFileFormat);
```

### Vedi anche

* class [SaveTemplateOptions](../)
* namespace [Aspose.Tasks.Saving](../../savetemplateoptions/)
* assembly [Aspose.Tasks](../../../)


