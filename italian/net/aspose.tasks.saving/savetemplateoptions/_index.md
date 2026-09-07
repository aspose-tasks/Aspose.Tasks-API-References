---
title: "Class SaveTemplateOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Saving.SaveTemplateOptions. Consente di specificare opzioni aggiuntive quando si salva un progetto come modello"
type: docs
weight: 2200
url: /it/net/aspose.tasks.saving/savetemplateoptions/
---
## SaveTemplateOptions class

Consente di specificare opzioni aggiuntive durante il salvataggio di un progetto come modello.

```csharp
public class SaveTemplateOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SaveTemplateOptions](savetemplateoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [RemoveActualValues](../../aspose.tasks.saving/savetemplateoptions/removeactualvalues/) { get; set; } | Ottiene o imposta un valore che indica se tutti i valori effettivi da un modello di progetto devono essere rimossi. |
| [RemoveBaselineValues](../../aspose.tasks.saving/savetemplateoptions/removebaselinevalues/) { get; set; } | Ottiene o imposta un valore che indica se tutti i valori di baseline da un modello di progetto devono essere rimossi. |
| [RemoveFixedCosts](../../aspose.tasks.saving/savetemplateoptions/removefixedcosts/) { get; set; } | Ottiene o imposta un valore che indica se tutti i costi fissi da un modello di progetto devono essere rimossi. |
| [RemoveResourceRates](../../aspose.tasks.saving/savetemplateoptions/removeresourcerates/) { get; set; } | Ottiene o imposta un valore che indica se le tariffe delle risorse da un modello di progetto devono essere rimosse. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


