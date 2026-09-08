---
title: "SaveOptions.UseGradientBrush"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad SaveOptions. Obtiene o establece un valor que indica si se debe usar el pincel de degradado al renderizar el diagrama de Gantt"
type: docs
weight: 220
url: /es/net/aspose.tasks.saving/saveoptions/usegradientbrush/
---
## SaveOptions.UseGradientBrush property

Obtiene o establece un valor que indica si se debe usar un pincel degradado al renderizar el diagrama de Gantt.

```csharp
public virtual bool UseGradientBrush { get; set; }
```

## Observaciones

Solo se aplica cuando se renderiza la vista de diagrama de Gantt.

## Ejemplos

muestra cómo establecer un valor que indica si se debe usar el pincel de degradado al renderizar el diagrama de Gantt.

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

### Ver también

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


