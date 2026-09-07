---
title: "HtmlSaveOptions.IncludeProjectNameInPageHeader"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà HtmlSaveOptions. Ottiene o imposta un valore che indica se includere il nome del progetto nell'intestazione della pagina HTML"
type: docs
weight: 110
url: /it/net/aspose.tasks.saving/htmlsaveoptions/includeprojectnameinpageheader/
---
## HtmlSaveOptions.IncludeProjectNameInPageHeader property

Ottiene o imposta un valore che indica se includere il nome del progetto nell'intestazione della pagina HTML.

```csharp
public bool IncludeProjectNameInPageHeader { get; set; }
```

## Esempi

Mostra come impostare l'intestazione/titolo della pagina HTML utilizzando le opzioni &lt;see cref=\"P:Aspose.Tasks.Saving.HtmlSaveOptions\" /&gt;.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new HtmlSaveOptions
{
    // Determina se includere il nome del progetto nel titolo HTML (true per impostazione predefinita)
    IncludeProjectNameInTitle = false,

    // Determina se includere il nome del progetto nell'intestazione della pagina HTML (true per impostazione predefinita)
    IncludeProjectNameInPageHeader = false,

    // imposta le pagine da esportare
    Pages = new List<int>
            {
                1
            }
};
project.Save(OutDir + "ControlHeaderNameDuringHTMLExport_out.html", options);
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


