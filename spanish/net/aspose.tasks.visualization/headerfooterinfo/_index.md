---
title: "Clase HeaderFooterInfo"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Visualization.HeaderFooterInfo. Representa el contenido visual del encabezado, pie de página o leyenda que se utiliza para la impresión y renderizado de vistas"
type: docs
weight: 3130
url: /es/net/aspose.tasks.visualization/headerfooterinfo/
---
## HeaderFooterInfo class

Representa el contenido visual del encabezado, pie de página o leyenda que se usa para la impresión \ renderizado de vistas.

```csharp
public class HeaderFooterInfo
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [HeaderFooterInfo](headerfooterinfo/)() | Inicializa una nueva instancia de la clase `HeaderFooterInfo`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | Obtiene o establece la imagen centrada que se mostrará en el elemento padre. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | Obtiene o establece el tamaño mostrado de la imagen central. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | Obtiene o establece el texto centrado que se mostrará en el elemento padre. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | Obtiene o establece la imagen alineada a la izquierda que se mostrará en el elemento padre. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | Obtiene o establece el tamaño mostrado de la imagen izquierda. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | Obtiene o establece el texto alineado a la izquierda que se mostrará en el elemento padre. |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | Obtiene o establece la imagen alineada a la derecha que se mostrará en el elemento padre. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | Obtiene o establece el tamaño mostrado de la imagen derecha. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | Obtiene o establece el texto alineado a la derecha que se mostrará en el elemento padre. |

## Ejemplos

Muestra cómo leer la información del encabezado/pie de página.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var info = project.DefaultView.PageInfo;

Console.WriteLine("Header left text: {0} ", info.Header.LeftText);
Console.WriteLine("Header left image: {0} ", info.Header.LeftImage);
Console.WriteLine("Header left image size: {0} ", info.Header.LeftImageSize);
Console.WriteLine("Header center text: {0} ", info.Header.CenteredText);
Console.WriteLine("Header center image: {0} ", info.Header.CenteredImage);
Console.WriteLine("Header center image size: {0} ", info.Header.CenteredImageSize);
Console.WriteLine("Header right text: {0} ", info.Header.RightText);
Console.WriteLine("Header right image: {0} ", info.Header.RightImage);
Console.WriteLine("Header right image size: {0} ", info.Header.RightImageSize);
Console.WriteLine();
Console.WriteLine("Footer left text: {0} ", info.Footer.LeftText);
Console.WriteLine("Footer left image: {0} ", info.Footer.LeftImage);
Console.WriteLine("Footer left image size: {0} ", info.Footer.LeftImageSize);
Console.WriteLine("Footer center text: {0} ", info.Footer.CenteredText);
Console.WriteLine("Footer center image: {0} ", info.Footer.CenteredImage);
Console.WriteLine("Footer center size: {0} ", info.Footer.CenteredImageSize);
Console.WriteLine("Footer right text: {0} ", info.Footer.RightText);
Console.WriteLine("Footer right image: {0} ", info.Footer.RightImage);
Console.WriteLine("Footer right image size: {0} ", info.Footer.RightImageSize);
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


