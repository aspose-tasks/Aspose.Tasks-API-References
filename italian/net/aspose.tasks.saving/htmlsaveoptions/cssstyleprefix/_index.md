---
title: "HtmlSaveOptions.CssStylePrefix"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà HtmlSaveOptions. Ottiene o imposta il prefisso di stile CSS"
type: docs
weight: 30
url: /it/net/aspose.tasks.saving/htmlsaveoptions/cssstyleprefix/
---
## HtmlSaveOptions.CssStylePrefix property

Ottiene o imposta il prefisso dello stile CSS.

```csharp
public string CssStylePrefix { get; set; }
```

## Esempi

Mostra come impostare un prefisso comune per gli stili CSS utilizzati durante l'esportazione in HTML.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new HtmlSaveOptions { CssStylePrefix = "test_prefix" };

project.Save(OutDir + "TestCssStylePrefix_out.html", options);
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


