---
title: "HtmlSaveOptions.HtmlSaveOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "HtmlSaveOptions constructor. Initialiseert een nieuw exemplaar van de HtmlSaveOptions klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks.saving/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions constructor

Initialiseert een nieuw exemplaar van de [`HtmlSaveOptions`](../) klasse.

```csharp
public HtmlSaveOptions()
```

## Voorbeelden

Toont hoe een project op te slaan in HTML‑formaat.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var option = new HtmlSaveOptions();
project.Save(OutDir + "SaveProjectDataAsHTML_out.html", option);

// OF

// Alleen één pagina toevoegen (paginanummer 2)
option = new HtmlSaveOptions();
option.Pages.Add(2);
project.Save(OutDir + "SaveProjectDataAsHTML2_out.html", option);
```

### Zie ook

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


