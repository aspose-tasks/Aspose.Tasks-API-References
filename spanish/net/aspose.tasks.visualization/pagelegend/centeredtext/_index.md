---
title: "PageLegend.CenteredText"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PageLegend. Obtiene o establece el texto centrado que se mostrará en la leyenda de la página."
type: docs
weight: 30
url: /es/net/aspose.tasks.visualization/pagelegend/centeredtext/
---
## PageLegend.CenteredText property

Obtiene o establece el texto centrado que se mostrará en la leyenda de la página.

```csharp
public string CenteredText { get; set; }
```

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

### Ver también

* class [PageLegend](../)
* namespace [Aspose.Tasks.Visualization](../../pagelegend/)
* assembly [Aspose.Tasks](../../../)


