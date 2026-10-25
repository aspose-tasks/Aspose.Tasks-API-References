---
title: "ProjectView.GetDefaultResourceSheetView"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectView-methode. Bevat kolommen Uid, resource-naam, type, materiaal, label, initialen, groep, max eenheden, standaardtarief, overurenttarief, kosten per gebruik, opbouw bij basisagenda en code resource"
type: docs
weight: 40
url: /nl/net/aspose.tasks.visualization/projectview/getdefaultresourcesheetview/
---
## ProjectView.GetDefaultResourceSheetView method

Bevat Uid-, resource-naam-, type-, materiaallabel-, initialen-, groep-, max eenheden-, standaardtarief-, overurenttarief-, kosten per gebruik-, opbouw bij-, basisagenda- en code-resourcekolommen.

```csharp
public static ProjectView GetDefaultResourceSheetView()
```

### Retourwaarde

een weergave die een lijst bevat van [`ResourceViewColumn`](../../resourceviewcolumn/).

## Voorbeelden

Toont hoe je een project opslaat met de resourcebladweergave.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceSheetView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceSheetView_out.pdf", options);
```

### Zie ook

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


