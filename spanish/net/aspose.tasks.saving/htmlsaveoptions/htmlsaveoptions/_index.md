---
title: "HtmlSaveOptions.HtmlSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor HtmlSaveOptions. Inicializa una nueva instancia de la clase HtmlSaveOptions"
type: docs
weight: 10
url: /es/net/aspose.tasks.saving/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions constructor

Inicializa una nueva instancia de la clase [`HtmlSaveOptions`](../).

```csharp
public HtmlSaveOptions()
```

## Ejemplos

Muestra cómo guardar un proyecto en formato HTML.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var option = new HtmlSaveOptions();
project.Save(OutDir + "SaveProjectDataAsHTML_out.html", option);

// O

// Añadiendo solo una página (número de página 2)
option = new HtmlSaveOptions();
option.Pages.Add(2);
project.Save(OutDir + "SaveProjectDataAsHTML2_out.html", option);
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


