---
title: "XamlOptions.XamlOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de XamlOptions. Inicializa una nueva instancia de la clase XamlOptions que puede usarse para guardar el proyecto en formato XAML"
type: docs
weight: 10
url: /es/net/aspose.tasks.saving/xamloptions/xamloptions/
---
## XamlOptions constructor

Inicializa una nueva instancia de la clase [`XamlOptions`](../) que puede usarse para guardar el proyecto en formato XAML.

```csharp
public XamlOptions()
```

## Ejemplos

Muestra cómo guardar un proyecto en formato XAML usando opciones de guardado.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new XamlOptions();
options.FitContent = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.Timescale = Timescale.ThirdsOfMonths;
project.Save(OutDir + "RenderXAMLWithOptions_out.xaml", options);
```

### Ver también

* class [XamlOptions](../)
* namespace [Aspose.Tasks.Saving](../../xamloptions/)
* assembly [Aspose.Tasks](../../../)


