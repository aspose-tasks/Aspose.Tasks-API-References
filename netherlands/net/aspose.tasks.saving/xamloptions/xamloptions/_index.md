---
title: "XamlOptions.XamlOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "XamlOptions constructor. Initialiseert een nieuw exemplaar van de XamlOptions-klasse die kan worden gebruikt om een project op te slaan in XAML-indeling"
type: docs
weight: 10
url: /nl/net/aspose.tasks.saving/xamloptions/xamloptions/
---
## XamlOptions constructor

Initialiseert een nieuw exemplaar van de [`XamlOptions`](../) klasse die kan worden gebruikt om een project op te slaan in XAML-indeling.

```csharp
public XamlOptions()
```

## Voorbeelden

Toont hoe een project op te slaan in XAML-indeling met behulp van opslaan‑opties.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new XamlOptions();
options.FitContent = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "RenderXAMLWithOptions_out.xaml", options);
```

### Zie ook

* class [XamlOptions](../)
* namespace [Aspose.Tasks.Saving](../../xamloptions/)
* assembly [Aspose.Tasks](../../../)


