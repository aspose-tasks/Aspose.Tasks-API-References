---
title: "PageInfo.Legend"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PageInfo. Obtiene o establece una instancia de la clase PageLegend que especifica las opciones de renderizado de la leyenda de página"
type: docs
weight: 40
url: /es/net/aspose.tasks.visualization/pageinfo/legend/
---
## PageInfo.Legend property

Obtiene o establece una instancia de la clase [`PageLegend`](../../pagelegend/) que especifica las opciones de renderizado de la leyenda de página.

```csharp
public PageLegend Legend { get; set; }
```

## Observaciones

Actualmente solo es aplicable a vistas de diagrama de Gantt.

## Ejemplos

Muestra cómo trabajar con la información de la leyenda de página.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// leamos la información de la leyenda de página
var legend = project.DefaultView.PageInfo.Legend;

Console.WriteLine("Legend left text: {0} ", legend.LeftText);
Console.WriteLine("Legend left image: {0} ", legend.LeftImage);
Console.WriteLine("Legend center text: {0} ", legend.CenteredText);
Console.WriteLine("Legend center image: {0} ", legend.CenteredImage);
Console.WriteLine("Legend right text: {0} ", legend.RightText);
Console.WriteLine("Legend right image: {0} ", legend.RightImage);
Console.WriteLine("Legend On: {0} ", legend.LegendOn);
Console.WriteLine("Legend Width: {0} ", legend.Width);

// también se admite la modificación de una leyenda
legend.LeftText = "New Left Text";

project.Save(OutDir + "WorkWithPageLegend_out.mpp", SaveFileFormat.Mpp);
```

Muestra cómo trabajar con la información de página de la vista de MS Project.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// permite modificar la vista predeterminada
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// permite modificar los márgenes
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// modifiquemos la configuración de página
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// modifiquemos la configuración de vista de página
// establece un valor que indica si se imprimen notas.
info.PageViewSettings.PrintNotes = true;

var header = new HeaderFooterInfo
{
    LeftText = "Left header text",
    CenteredText = "Centered header text",
    RightText = "Right header text"
};
var legend = new PageLegend
{
    LeftText =  "Left legend text",
    CenteredText = "Centered legend text",
    RightText = "Right legend text"
};
var footer = new HeaderFooterInfo
{
    LeftText = "Left footer text",
    CenteredText = "Centered footer text",
    RightText = "Right footer text"
};

info.Header = header;
info.Legend = legend;
info.Footer = footer;

// trabajar con el proyecto...
```

### Ver también

* class [PageLegend](../../pagelegend/)
* class [PageInfo](../)
* namespace [Aspose.Tasks.Visualization](../../pageinfo/)
* assembly [Aspose.Tasks](../../../)


