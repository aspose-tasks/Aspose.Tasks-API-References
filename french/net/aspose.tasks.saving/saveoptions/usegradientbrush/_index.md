---
title: "SaveOptions.UseGradientBrush"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SaveOptions. Obtient ou définit une valeur indiquant si le pinceau dégradé doit être utilisé lors du rendu du diagramme de Gantt"
type: docs
weight: 220
url: /fr/net/aspose.tasks.saving/saveoptions/usegradientbrush/
---
## SaveOptions.UseGradientBrush property

Obtient ou définit une valeur indiquant si un pinceau dégradé doit être utilisé lors du rendu du diagramme de Gantt.

```csharp
public virtual bool UseGradientBrush { get; set; }
```

## Remarques

Ne s'applique que lorsque la vue du diagramme de Gantt est rendue.

## Exemples

Montre comment définir une valeur indiquant si le pinceau dégradé doit être utilisé lors du rendu du diagramme de Gantt.

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

### Voir aussi

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


