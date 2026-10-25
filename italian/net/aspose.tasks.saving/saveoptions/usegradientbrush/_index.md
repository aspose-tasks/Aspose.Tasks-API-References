---
title: "SaveOptions.UseGradientBrush"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà SaveOptions. Ottiene o imposta un valore che indica se il pennello gradiente deve essere utilizzato durante il rendering del diagramma di Gantt"
type: docs
weight: 220
url: /it/net/aspose.tasks.saving/saveoptions/usegradientbrush/
---
## SaveOptions.UseGradientBrush property

Ottiene o imposta un valore che indica se deve essere utilizzato un pennello gradiente durante il rendering del diagramma di Gantt.

```csharp
public virtual bool UseGradientBrush { get; set; }
```

## Osservazioni

È applicabile solo quando la vista del diagramma di Gantt viene renderizzata.

## Esempi

mostra come impostare un valore che indica se il pennello gradiente deve essere utilizzato durante il rendering del diagramma di Gantt.

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

### Vedi anche

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


