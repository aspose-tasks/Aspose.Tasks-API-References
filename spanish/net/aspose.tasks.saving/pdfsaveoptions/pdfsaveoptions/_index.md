---
title: "PdfSaveOptions.PdfSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor PdfSaveOptions. Inicializa una nueva instancia de la clase PdfSaveOptions que puede usarse para guardar un documento en formato PDF"
type: docs
weight: 10
url: /es/net/aspose.tasks.saving/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

Inicializa una nueva instancia de la clase [`PdfSaveOptions`](../) que puede usarse para guardar un documento en el formato [`PDF`](../../savefileformat/).

```csharp
public PdfSaveOptions()
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


