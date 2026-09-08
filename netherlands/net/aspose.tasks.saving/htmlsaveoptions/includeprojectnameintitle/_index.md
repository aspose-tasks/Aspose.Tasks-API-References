---
title: "HtmlSaveOptions.IncludeProjectNameInTitle"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "HtmlSaveOptions eigenschap. Haalt een waarde op of stelt deze in die aangeeft of de projectnaam moet worden opgenomen in de HTML-titel."
type: docs
weight: 120
url: /nl/net/aspose.tasks.saving/htmlsaveoptions/includeprojectnameintitle/
---
## HtmlSaveOptions.IncludeProjectNameInTitle property

Haalt op of stelt een waarde in die aangeeft of de projectnaam moet worden opgenomen in de HTML‑titel.

```csharp
public bool IncludeProjectNameInTitle { get; set; }
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


