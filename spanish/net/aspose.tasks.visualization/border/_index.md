---
title: "Enum Border"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Visualization.Border enum. Especifica el tipo de bordes"
type: docs
weight: 2970
url: /es/net/aspose.tasks.visualization/border/
---
## Border enumeration

Especifica los bordes del tipo.

```csharp
public enum Border
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| NoBorder | `0` | Sin borde. |
| AroundEveryPage | `1` | Alrededor de cada página. |
| OutsidePages | `2` | En las páginas externas. |

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


