---
title: "HtmlSaveOptions.HtmlSaveOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore HtmlSaveOptions. Inizializza una nuova istanza della classe HtmlSaveOptions"
type: docs
weight: 10
url: /it/net/aspose.tasks.saving/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions constructor

Inizializza una nuova istanza della classe [`HtmlSaveOptions`](../).

```csharp
public HtmlSaveOptions()
```

## Esempi

Mostra come salvare un progetto in formato HTML.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var option = new HtmlSaveOptions();
project.Save(OutDir + "SaveProjectDataAsHTML_out.html", option);

// OPPURE

// Aggiunta di una sola pagina (numero pagina 2)
option = new HtmlSaveOptions();
option.Pages.Add(2);
project.Save(OutDir + "SaveProjectDataAsHTML2_out.html", option);
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


