---
title: "XamlOptions.XamlOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur XamlOptions. Initialise une nouvelle instance de la classe XamlOptions qui peut être utilisée pour enregistrer le projet au format XAML"
type: docs
weight: 10
url: /fr/net/aspose.tasks.saving/xamloptions/xamloptions/
---
## XamlOptions constructor

Initialise une nouvelle instance de la classe [`XamlOptions`](../) qui peut être utilisée pour enregistrer le projet au format XAML.

```csharp
public XamlOptions()
```

## Exemples

Montre comment enregistrer un projet au format XAML en utilisant les options d'enregistrement.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new XamlOptions();
options.FitContent = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "RenderXAMLWithOptions_out.xaml", options);
```

### Voir aussi

* class [XamlOptions](../)
* namespace [Aspose.Tasks.Saving](../../xamloptions/)
* assembly [Aspose.Tasks](../../../)


