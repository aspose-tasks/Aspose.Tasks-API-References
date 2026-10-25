---
title: "PageMargins.Right"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PageMargins. Obtiene o establece el tamaño del margen derecho en centímetros"
type: docs
weight: 50
url: /es/net/aspose.tasks.visualization/pagemargins/right/
---
## PageMargins.Right property

Obtiene o establece el tamaño del margen derecho en centímetros.

```csharp
public double Right { get; set; }
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


