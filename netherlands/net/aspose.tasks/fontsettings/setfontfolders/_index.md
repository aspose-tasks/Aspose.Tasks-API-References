---
title: "FontSettings.SetFontFolders"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "FontSettings methode. Stelt de mappen in waar Aspose.Tasks zoekt naar TrueType-lettertypen bij het renderen van de projectweergave"
type: docs
weight: 50
url: /nl/net/aspose.tasks/fontsettings/setfontfolders/
---
## FontSettings.SetFontFolders method

Stelt de mappen in waarin Aspose.Tasks zoekt naar TrueType‑lettertypen bij het renderen van de projectweergave.

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fontFolders | String[] | Een array van mappen die TrueType-lettertypen bevatten. |
| recursive | Boolean | Als true worden de opgegeven mappen recursief gescand. |

## Voorbeelden

Toont hoe een aangepaste lettertype‑map in te stellen.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

// TrueType-lettertypebestanden voor alle lettertypen die in het geopende project worden gebruikt, moeten zich bevinden in de map MyFonts.
options.FontSettings.SetFontFolders(new string[] { "c:\\MyFonts"}, true);

project.Save(OutDir + "EstimatedMilestoneTasks_out4.pdf", options);
```

### Zie ook

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


