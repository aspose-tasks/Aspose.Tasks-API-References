---
title: "ProjectView.GetDefaultResourceUsageView"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ProjectView-methode. Bevat Uid naam start eind en werk resourcekolommen"
type: docs
weight: 50
url: /nl/net/aspose.tasks.visualization/projectview/getdefaultresourceusageview/
---
## ProjectView.GetDefaultResourceUsageView method

Bevat Uid, naam, start, eind en werkresourcekolommen.

```csharp
public static ProjectView GetDefaultResourceUsageView()
```

### Retourwaarde

een weergave die een lijst bevat van [`ResourceViewColumn`](../../resourceviewcolumn/).

## Voorbeelden

Toont hoe een project op te slaan met resourcegebruikweergave.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceUsageView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceUsageView_out.pdf", options);
```

### Zie ook

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


