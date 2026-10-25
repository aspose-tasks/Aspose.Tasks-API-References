---
title: "FontSettings.DefaultFontName"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété FontSettings. Obtient ou définit la police par défaut ou de secours pour le rendu"
type: docs
weight: 20
url: /fr/net/aspose.tasks/fontsettings/defaultfontname/
---
## FontSettings.DefaultFontName property

Obtient ou définit la police par défaut (ou de secours) pour le rendu.

```csharp
public string DefaultFontName { get; set; }
```

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


