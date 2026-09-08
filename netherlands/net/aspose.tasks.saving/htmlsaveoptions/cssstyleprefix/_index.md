---
title: "HtmlSaveOptions.CssStylePrefix"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "HtmlSaveOptions eigenschap. Haalt het CSS‑stijlprefix op of stelt het in"
type: docs
weight: 30
url: /nl/net/aspose.tasks.saving/htmlsaveoptions/cssstyleprefix/
---
## HtmlSaveOptions.CssStylePrefix property

Haalt op of stelt het CSS-stijlprefix in.

```csharp
public string CssStylePrefix { get; set; }
```

## Voorbeelden

Toont hoe een gemeenschappelijk prefix voor CSS‑stijlen in te stellen die tijdens export naar HTML worden gebruikt.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new HtmlSaveOptions { CssStylePrefix = "test_prefix" };

project.Save(OutDir + "TestCssStylePrefix_out.html", options);
```

### Zie ook

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


