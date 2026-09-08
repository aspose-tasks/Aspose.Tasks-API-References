---
title: "PageSettings.PagesInWidth"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PageSettings. Obtiene o establece un número de páginas en ancho que se imprimirán"
type: docs
weight: 60
url: /es/net/aspose.tasks.visualization/pagesettings/pagesinwidth/
---
## PageSettings.PagesInWidth property

Obtiene o establece la cantidad de páginas en anchura que se imprimirán.

```csharp
public int PagesInWidth { get; set; }
```

## Ejemplos

Muestra cómo renderizar la vista con la opción 'Ajustar X a Y páginas'.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.TaskUsage);

view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = false;
// especifica que la vista debe renderizarse en 2 páginas o menos en altura
view.PageInfo.PageSettings.PagesInHeight = 2;
// especifica que la vista debe renderizarse en 1 página en ancho
view.PageInfo.PageSettings.PagesInWidth = 1;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView,
    StartDate =  new DateTime(2000, 04, 1),
    EndDate = new DateTime(2000, 12, 31)
};

project.Save(OutDir + "PrintViewWithFitToPages_out.pdf", saveOptions);
```

### Ver también

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


