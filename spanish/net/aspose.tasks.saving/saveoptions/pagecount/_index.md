---
title: "SaveOptions.PageCount"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad SaveOptions. Obtiene o establece el número de páginas del proyecto."
type: docs
weight: 120
url: /es/net/aspose.tasks.saving/saveoptions/pagecount/
---
## SaveOptions.PageCount property

Obtiene o establece el número de páginas del proyecto.

```csharp
public int PageCount { get; }
```

## Ejemplos

Muestra cómo guardar páginas seleccionadas de un proyecto en un archivo PDF.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// verifiquemos cuántas páginas se pueden exportar
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### Ver también

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


