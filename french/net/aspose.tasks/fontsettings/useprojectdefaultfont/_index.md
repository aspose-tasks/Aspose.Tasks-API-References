---
title: "FontSettings.UseProjectDefaultFont"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété FontSettings. Obtient ou définit une valeur indiquant si la police par défaut doit être utilisée pour le rendu"
type: docs
weight: 40
url: /fr/net/aspose.tasks/fontsettings/useprojectdefaultfont/
---
## FontSettings.UseProjectDefaultFont property

Obtient ou définit une valeur indiquant si la police par défaut doit être utilisée pour le rendu.

```csharp
public bool UseProjectDefaultFont { get; set; }
```

## Remarques

Lorsque la valeur est False et que DefaultFontName est spécifié, le moteur de rendu utilisera la police indiquée par DefaultFontName comme police de secours. Sinon, les polices 'Arial' (si installée) ou 'Generic Sans Serif' sont utilisées comme police de secours. La police de secours est utilisée lors du rendu de la vue du projet lorsqu'un style de texte fait référence à une police qui n'est pas installée sur le système d'exploitation actuel. Pour un contrôle plus fin de la résolution des polices, vous pouvez utiliser le rappel [`FontResolveCallback`](../fontresolvecallback/).

## Exemples

Montre comment définir une police personnalisée qui sera utilisée pour l'impression du PDF de sortie.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart, FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "CreateProject2_out.pdf", options);
```

### Voir aussi

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


