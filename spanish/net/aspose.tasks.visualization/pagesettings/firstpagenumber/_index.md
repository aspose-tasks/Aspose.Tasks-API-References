---
title: "PageSettings.FirstPageNumber"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PageSettings. Obtiene o establece el número de la primera página para la impresión"
type: docs
weight: 30
url: /es/net/aspose.tasks.visualization/pagesettings/firstpagenumber/
---
## PageSettings.FirstPageNumber property

Obtiene o establece el número de la primera página para imprimir.

```csharp
public short FirstPageNumber { get; set; }
```

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

### Ver también

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


