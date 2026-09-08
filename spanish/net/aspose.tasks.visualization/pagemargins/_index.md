---
title: "Clase PageMargins"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Visualization.PageMargins. Representa los márgenes de página para impresión"
type: docs
weight: 3230
url: /es/net/aspose.tasks.visualization/pagemargins/
---
## PageMargins class

Representa los márgenes de página para la impresión.

```csharp
public class PageMargins
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PageMargins](pagemargins/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Borders](../../aspose.tasks.visualization/pagemargins/borders/) { get; set; } | Obtiene o establece una posición donde imprimir los bordes. Puede ser uno de los valores de la enumeración [`Border`](../border/). |
| [Bottom](../../aspose.tasks.visualization/pagemargins/bottom/) { get; set; } | Obtiene o establece el tamaño del margen inferior en centímetros. |
| [Left](../../aspose.tasks.visualization/pagemargins/left/) { get; set; } | Obtiene o establece el tamaño del margen izquierdo en centímetros. |
| [Right](../../aspose.tasks.visualization/pagemargins/right/) { get; set; } | Obtiene o establece el tamaño del margen derecho en centímetros. |
| [Top](../../aspose.tasks.visualization/pagemargins/top/) { get; set; } | Obtiene o establece el tamaño del margen superior en centímetros. |

## Ejemplos

Muestra cómo trabajar con los márgenes de página.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// permite modificar la vista predeterminada
var margins = project.DefaultView.PageInfo.Margins;

// permite modificar los márgenes
margins.Left = 10d;
margins.Top = 10d;
margins.Right = 10d;
margins.Bottom = 10d;
margins.Borders = Border.OutsidePages;

project.Save(OutDir + "WorkWithPageMargins_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


