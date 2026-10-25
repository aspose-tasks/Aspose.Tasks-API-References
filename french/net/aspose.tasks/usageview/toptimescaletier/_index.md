---
title: "UsageView.TopTimescaleTier"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété UsageView. Obtient ou définit les paramètres du niveau d'échelle de temps supérieur des vues. TimescaleTier"
type: docs
weight: 80
url: /fr/net/aspose.tasks/usageview/toptimescaletier/
---
## UsageView.TopTimescaleTier property

Obtient ou définit les paramètres du niveau d'échelle de temps supérieur de la vue. [`TimescaleTier`](../../../aspose.tasks.visualization/timescaletier/).

```csharp
public TimescaleTier TopTimescaleTier { get; set; }
```

## Exemples

Montre comment rendre la vue d'utilisation des tâches avec les paramètres d'échelle de temps définis dans les paramètres de vue.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// Définissez les SaveOptions et spécifiez que les paramètres d'échelle de temps TaskUsageView doivent être utilisés.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

### Voir aussi

* class [TimescaleTier](../../../aspose.tasks.visualization/timescaletier/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


