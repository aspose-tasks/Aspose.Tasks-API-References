---
title: "PageMargins.Borders"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PageMargins. Obtiene o establece una posición donde imprimir los bordes. Puede ser uno de los valores de la enumeración Border"
type: docs
weight: 20
url: /es/net/aspose.tasks.visualization/pagemargins/borders/
---
## PageMargins.Borders property

Obtiene o establece una posición donde imprimir los bordes. Puede ser uno de los valores de la enumeración [`Border`](../../border/).

```csharp
public Border Borders { get; set; }
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

* enum [Border](../../border/)
* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


