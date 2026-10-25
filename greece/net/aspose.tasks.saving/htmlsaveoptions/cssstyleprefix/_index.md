---
title: "HtmlSaveOptions.CssStylePrefix"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα HtmlSaveOptions. Λαμβάνει ή ορίζει το πρόθεμα στυλ CSS"
type: docs
weight: 30
url: /el/net/aspose.tasks.saving/htmlsaveoptions/cssstyleprefix/
---
## HtmlSaveOptions.CssStylePrefix property

Λαμβάνει ή ορίζει το πρόθεμα στυλ CSS.

```csharp
public string CssStylePrefix { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε ένα κοινό πρόθεμα για τα στυλ CSS που χρησιμοποιούνται κατά την εξαγωγή σε HTML.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new HtmlSaveOptions { CssStylePrefix = "test_prefix" };

project.Save(OutDir + "TestCssStylePrefix_out.html", options);
```

### Δείτε επίσης

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


