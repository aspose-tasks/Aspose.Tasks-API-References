---
title: "HtmlSaveOptions.Pages"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà HtmlSaveOptions. Ottiene o imposta un elenco di numeri di pagina da salvare durante il rendering del layout del progetto. Tutte le pagine del progetto verranno salvate se questo elenco è vuoto"
type: docs
weight: 130
url: /it/net/aspose.tasks.saving/htmlsaveoptions/pages/
---
## HtmlSaveOptions.Pages property

Ottiene o imposta un elenco di numeri di pagina da salvare durante il rendering del layout del progetto. Tutte le pagine del progetto saranno salvate se questo elenco è vuoto.

```csharp
public List<int> Pages { get; set; }
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


