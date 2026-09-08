---
title: "PageSettings.IsPortrait"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PageSettings. Obtiene o establece un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal"
type: docs
weight: 40
url: /es/net/aspose.tasks.visualization/pagesettings/isportrait/
---
## PageSettings.IsPortrait property

Obtiene o establece un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal.

```csharp
public bool IsPortrait { get; set; }
```

## Observaciones

Es aplicable durante el renderizado cuando SaveOptions.PageSize == Visualization.PageSize.DefinedInView.

## Ejemplos

Muestra cómo trabajar con &lt;see cref=\"Aspose.Tasks.Visualization.PageSettings\" /&gt;.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// obtener la configuración
var settings = project.DefaultView.PageInfo.PageSettings;
// ajustemos algunas propiedades
// establece un valor que indica si la orientación de la página es vertical; devuelve false si la orientación de la página es horizontal.
settings.IsPortrait = true;
// establece la cantidad de páginas en anchura que se imprimirán.
settings.PagesInWidth = 5;
// establece la cantidad de páginas en altura que se imprimirán.
settings.PagesInHeight = 7;
// establece un porcentaje del tamaño normal al que se debe ajustar la impresión.
settings.PercentOfNormalSize = 200;
// establece un tamaño de papel. Puede ser uno de los valores de la enumeración <see cref=\"T:Aspose.Tasks.Visualization.PrinterPaperSize\" />.
settings.PaperSize = PrinterPaperSize.PaperB4;
// establece el número de la primera página para imprimir.
settings.FirstPageNumber = 3;

SimpleSaveOptions options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "TestCanWritePageSettings.mpp", options);
```

Muestra cómo especificar el tamaño y la orientación de la página usando la configuración View o usando SaveOptions.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

saveOptions.PageSize = PageSize.DefinedInView;

// En este caso, el tamaño y la orientación de la página se aplican a partir de las propiedades view.PageInfo.PageSettings.PaperSize y view.PageInfo.PageSettings.IsPortrait.
project.Save(OutDir + "WorkWithIsPortrait_out1.pdf", saveOptions);

saveOptions.PageSize = PageSize.A4;
saveOptions.IsPortrait = true;

// En este caso, el tamaño y la orientación de la página se aplican a partir de las propiedades de SaveOptions.
project.Save(OutDir + "WorkWithIsPortrait_out2.pdf", saveOptions);

saveOptions.CustomPageSize = new SizeF(400, 600);

// En este caso, el tamaño de la página se aplica a partir de SaveOptions.CustomPageSize. La propiedad IsPortrait no se tiene en cuenta.
project.Save(OutDir + "WorkWithIsPortrait_out3.pdf", saveOptions);
```

### Ver también

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


