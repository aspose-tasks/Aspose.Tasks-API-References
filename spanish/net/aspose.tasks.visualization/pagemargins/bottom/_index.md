---
title: "PageMargins.Bottom"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PageMargins. Obtiene o establece el tamaño del margen inferior en centímetros"
type: docs
weight: 30
url: /es/net/aspose.tasks.visualization/pagemargins/bottom/
---
## PageMargins.Bottom property

Obtiene o establece el tamaño del margen inferior en centímetros.

```csharp
public double Bottom { get; set; }
```

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

* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


