---
title: "SaveOptions.NonWorkingTimeColor"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει το χρώμα μη εργάσιμου χρόνου."
type: docs
weight: 110
url: /el/net/aspose.tasks.saving/saveoptions/nonworkingtimecolor/
---
## SaveOptions.NonWorkingTimeColor property

Αποκτά ή ορίζει το χρώμα του μη εργάσιμου χρόνου.

```csharp
public Color NonWorkingTimeColor { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε προσαρμοσμένο χρώμα για μη εργάσιμο χρόνο.

```csharp
var project = new Project(DataDir + "ReadCurrencyProperties.mpp");
SaveOptions options = new PdfSaveOptions { NonWorkingTimeColor = Color.LightGray };
project.Save(OutDir + "ReadCurrencyProperties_out.pdf", options);
```

### Δείτε επίσης

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


