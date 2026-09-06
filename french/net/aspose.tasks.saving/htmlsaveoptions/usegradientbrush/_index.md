---
title: "HtmlSaveOptions.UseGradientBrush"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété HtmlSaveOptions. Obtient ou définit une valeur indiquant s'il faut utiliser un pinceau en dégradé lors du rendu de la mise en page du projet. L'utilisation du pinceau en dégradé n'est actuellement pas prise en charge lors du rendu en HTML."
type: docs
weight: 160
url: /fr/net/aspose.tasks.saving/htmlsaveoptions/usegradientbrush/
---
## HtmlSaveOptions.UseGradientBrush property

Obtient ou définit une valeur indiquant s'il faut utiliser un pinceau dégradé lors du rendu de la mise en page du projet. L'utilisation du pinceau dégradé n'est actuellement pas prise en charge lors du rendu en HTML.

```csharp
public override bool UseGradientBrush { get; set; }
```

## Exemples

Montre comment définir une police personnalisée qui sera utilisée pour exporter le projet dans un fichier HTML.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      PresentationFormat = PresentationFormat.GanttChart,
                      FitContent = true
                  };

options.FontSettings.UseProjectDefaultFont = false;
options.FontSettings.DefaultFontName = "Segoe UI Black";
project.Save(OutDir + "AddDefaultFontDuringSavingAsHtml_out.html", options);
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


