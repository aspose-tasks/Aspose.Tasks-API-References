---
title: "ProjectView.GetDefaultAssignmentView"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectView-methode. Bevat kolommen Uid, taaknaam, resource-naam, werk en duur voor toewijzingskolommen"
type: docs
weight: 20
url: /nl/net/aspose.tasks.visualization/projectview/getdefaultassignmentview/
---
## ProjectView.GetDefaultAssignmentView method

Bevat Uid-, taaknaam-, resource-naam-, werk- en duurtoewijzingskolommen.

```csharp
public static ProjectView GetDefaultAssignmentView()
```

### Retourwaarde

een weergave die een lijst bevat van [`AssignmentViewColumn`](../../assignmentviewcolumn/).

## Voorbeelden

Toont hoe een project op te slaan met de toewijzingsweergave.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultAssignmentView()
};

project.Save(OutDir + "WorkWithProjectView_AssignmentView_out.pdf", options);
```

### Zie ook

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


