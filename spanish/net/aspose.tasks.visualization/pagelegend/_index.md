---
title: "Clase PageLegend"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Visualization.PageLegend. Representa una leyenda de página que se usa para la impresión del proyecto."
type: docs
weight: 3210
url: /es/net/aspose.tasks.visualization/pagelegend/
---
## PageLegend class

Representa una leyenda de página que se usa para la impresión del proyecto.

```csharp
public class PageLegend : HeaderFooterInfo
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PageLegend](pagelegend/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | Obtiene o establece la imagen centrada que se mostrará en el elemento padre. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | Obtiene o establece el tamaño mostrado de la imagen central. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | Obtiene o establece el texto centrado que se mostrará en el elemento padre. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | Obtiene o establece la imagen alineada a la izquierda que se mostrará en el elemento padre. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | Obtiene o establece el tamaño mostrado de la imagen izquierda. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | Obtiene o establece el texto alineado a la izquierda que se mostrará en el elemento padre. |
| [LegendOn](../../aspose.tasks.visualization/pagelegend/legendon/) { get; set; } | Obtiene o establece las páginas en las que aparece la leyenda. Puede ser uno de los valores de la enumeración [`Legend`](../legend/). |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | Obtiene o establece la imagen alineada a la derecha que se mostrará en el elemento padre. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | Obtiene o establece el tamaño mostrado de la imagen derecha. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | Obtiene o establece el texto alineado a la derecha que se mostrará en el elemento padre. |
| [Width](../../aspose.tasks.visualization/pagelegend/width/) { get; set; } | Obtiene o establece el ancho de la parte izquierda (que contiene el nombre y la fecha del proyecto por defecto) de la leyenda en centímetros. |

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

* class [HeaderFooterInfo](../headerfooterinfo/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


