---
title: "HtmlSaveOptions.CssStylePrefix"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad HtmlSaveOptions. Obtiene o establece el prefijo de estilo CSS"
type: docs
weight: 30
url: /es/net/aspose.tasks.saving/htmlsaveoptions/cssstyleprefix/
---
## HtmlSaveOptions.CssStylePrefix property

Obtiene o establece el prefijo de estilo CSS.

```csharp
public string CssStylePrefix { get; set; }
```

## Ejemplos

Muestra cómo establecer un prefijo común para los estilos CSS que se utilizan durante la exportación a HTML.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new HtmlSaveOptions { CssStylePrefix = "test_prefix" };

project.Save(OutDir + "TestCssStylePrefix_out.html", options);
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


