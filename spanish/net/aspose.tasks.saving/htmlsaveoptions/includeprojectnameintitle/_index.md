---
title: "HtmlSaveOptions.IncludeProjectNameInTitle"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad HtmlSaveOptions. Obtiene o establece un valor que indica si se debe incluir el nombre del proyecto en el título HTML"
type: docs
weight: 120
url: /es/net/aspose.tasks.saving/htmlsaveoptions/includeprojectnameintitle/
---
## HtmlSaveOptions.IncludeProjectNameInTitle property

Obtiene o establece un valor que indica si se debe incluir el nombre del proyecto en el título HTML.

```csharp
public bool IncludeProjectNameInTitle { get; set; }
```

## Ejemplos

Muestra cómo establecer el encabezado/título HTML de la página usando las opciones &lt;see cref="P:Aspose.Tasks.Saving.HtmlSaveOptions" /&gt;.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new HtmlSaveOptions
{
    // Determina si se incluye el nombre del proyecto en el título HTML (true por defecto)
    IncludeProjectNameInTitle = false,

    // Determina si se incluye el nombre del proyecto en el encabezado de la página HTML (true por defecto)
    IncludeProjectNameInPageHeader = false,

    // establecer páginas que se exportarán
    Pages = new List<int>
            {
                1
            }
};
project.Save(OutDir + "ControlHeaderNameDuringHTMLExport_out.html", options);
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


