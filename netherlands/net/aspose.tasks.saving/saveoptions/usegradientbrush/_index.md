---
title: "SaveOptions.UseGradientBrush"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SaveOptions eigenschap. Haalt een waarde op of stelt deze in die aangeeft of een gradientkwast moet worden gebruikt bij het renderen van een Gantt-diagram"
type: docs
weight: 220
url: /nl/net/aspose.tasks.saving/saveoptions/usegradientbrush/
---
## SaveOptions.UseGradientBrush property

Haalt op of stelt een waarde in die aangeeft of een gradientkwast moet worden gebruikt bij het renderen van een Gantt-diagram.

```csharp
public virtual bool UseGradientBrush { get; set; }
```

## Opmerkingen

Is alleen van toepassing wanneer de Gantt‑chartweergave wordt gerenderd.

## Voorbeelden

toont hoe een waarde in te stellen die aangeeft of een gradientkwast moet worden gebruikt bij het renderen van een Gantt-diagram.

```csharp
var project = new Project(DataDir + "Project2.mpp");

SaveOptions options = new XamlOptions
{
    UseGradientBrush = false
};
project.Save(OutDir + "ChangeGanttBarsColorGradient_Solid_out.xaml", options);

options.UseGradientBrush = true;
project.Save(OutDir + "ChangeGanttBarsColorGradient_Gradient_out.xaml", options);
```

### Zie ook

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


