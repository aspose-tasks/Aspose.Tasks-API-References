---
title: "PdfSaveOptions.Pages"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PdfSaveOptions. Obtiene o establece la lista de números de página que se guardarán al guardar el diseño del proyecto en archivos separados. Todas las páginas se guardarán si esta lista está vacía."
type: docs
weight: 60
url: /es/net/aspose.tasks.saving/pdfsaveoptions/pages/
---
## PdfSaveOptions.Pages property

Obtiene o establece la lista de números de página a guardar al guardar el diseño del proyecto en archivos separados. Todas las páginas se guardarán si esta lista está vacía.

```csharp
public List<int> Pages { get; set; }
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

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


