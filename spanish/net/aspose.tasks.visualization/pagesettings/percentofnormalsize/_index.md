---
title: "PageSettings.PercentOfNormalSize"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PageSettings. Obtiene o establece un porcentaje del tamaño normal para ajustar la impresión a"
type: docs
weight: 90
url: /es/net/aspose.tasks.visualization/pagesettings/percentofnormalsize/
---
## PageSettings.PercentOfNormalSize property

Obtiene o establece un porcentaje del tamaño normal al que se debe ajustar la impresión.

```csharp
public int PercentOfNormalSize { get; set; }
```

## Ejemplos

Muestra cómo renderizar la vista con el factor de escala especificado.

```csharp
var project = new Project(DataDir + "Input.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

// establece un valor que indica que la vista debe escalarse usando el factor de escala especificado
view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = true;
// especifica el factor de escala
view.PageInfo.PageSettings.PercentOfNormalSize = 33;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "PrintViewWithSpecifiedScaleFactor_out.pdf", saveOptions);
```

### Ver también

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


