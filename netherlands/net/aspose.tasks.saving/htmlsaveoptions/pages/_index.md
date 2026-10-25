---
title: "HtmlSaveOptions.Pages"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "HtmlSaveOptions eigenschap. Haalt een lijst met paginanummers op of stelt deze in die moeten worden opgeslagen bij het renderen van de projectlay-out. Alle projectpagina's worden opgeslagen als deze lijst leeg is."
type: docs
weight: 130
url: /nl/net/aspose.tasks.saving/htmlsaveoptions/pages/
---
## HtmlSaveOptions.Pages property

Haalt op of stelt een lijst van paginanummers in die moeten worden opgeslagen bij het renderen van de projectlay-out. Alle projectpagina's worden opgeslagen als deze lijst leeg is.

```csharp
public List<int> Pages { get; set; }
```

## Voorbeelden

Toont hoe de HTML‑header/titel van een pagina in te stellen met behulp van &lt;see cref=\"P:Aspose.Tasks.Saving.HtmlSaveOptions\" /&gt; opties.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new HtmlSaveOptions
{
    // Bepaalt of de projectnaam in de HTML‑titel moet worden opgenomen (standaard true)
    IncludeProjectNameInTitle = false,

    // Bepaalt of de projectnaam in de HTML‑pagina‑header moet worden opgenomen (standaard true)
    IncludeProjectNameInPageHeader = false,

    // stel pagina's in die geëxporteerd zullen worden
    Pages = new List<int>
            {
                1
            }
};
project.Save(OutDir + "ControlHeaderNameDuringHTMLExport_out.html", options);
```

### Zie ook

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


