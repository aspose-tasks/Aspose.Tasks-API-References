---
title: "HtmlSaveOptions.HtmlSaveOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής HtmlSaveOptions. Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης HtmlSaveOptions"
type: docs
weight: 10
url: /el/net/aspose.tasks.saving/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions constructor

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`HtmlSaveOptions`](../).

```csharp
public HtmlSaveOptions()
```

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έργο σε μορφή HTML.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var option = new HtmlSaveOptions();
project.Save(OutDir + "SaveProjectDataAsHTML_out.html", option);

// Ή

// Προσθήκη μόνο μιας σελίδας (αριθμός σελίδας 2)
option = new HtmlSaveOptions();
option.Pages.Add(2);
project.Save(OutDir + "SaveProjectDataAsHTML2_out.html", option);
```

### Δείτε επίσης

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


