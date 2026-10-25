---
title: "PageLegend.Width"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PageLegend. Obtiene o establece el ancho de la parte izquierda que contiene el nombre y la fecha del proyecto por defecto de la leyenda en centímetros"
type: docs
weight: 30
url: /es/net/aspose.tasks.visualization/pagelegend/width/
---
## PageLegend.Width property

Obtiene o establece el ancho de la parte izquierda (que contiene el nombre y la fecha del proyecto por defecto) de la leyenda en centímetros.

```csharp
public double Width { get; set; }
```

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentOutOfRangeException | Al intentar establecer un valor menor que 0. |

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


