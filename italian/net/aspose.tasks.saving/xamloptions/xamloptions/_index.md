---
title: "XamlOptions.XamlOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore XamlOptions. Inizializza una nuova istanza della classe XamlOptions che può essere usata per salvare il progetto in formato XAML"
type: docs
weight: 10
url: /it/net/aspose.tasks.saving/xamloptions/xamloptions/
---
## XamlOptions constructor

Inizializza una nuova istanza della classe [`XamlOptions`](../) che può essere usata per salvare il progetto in formato XAML.

```csharp
public XamlOptions()
```

## Esempi

Mostra come salvare un progetto in formato XAML utilizzando le opzioni di salvataggio.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new XamlOptions();
options.FitContent = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "RenderXAMLWithOptions_out.xaml", options);
```

### Vedi anche

* class [XamlOptions](../)
* namespace [Aspose.Tasks.Saving](../../xamloptions/)
* assembly [Aspose.Tasks](../../../)


