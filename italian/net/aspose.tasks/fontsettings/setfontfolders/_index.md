---
title: "FontSettings.SetFontFolders"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo FontSettings. Imposta le cartelle in cui Aspose.Tasks cerca i font TrueType durante il rendering della vista dei progetti"
type: docs
weight: 50
url: /it/net/aspose.tasks/fontsettings/setfontfolders/
---
## FontSettings.SetFontFolders method

Imposta le cartelle in cui Aspose.Tasks cerca i caratteri TrueType durante il rendering della vista del progetto.

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontFolders | String[] | Un array di cartelle che contengono font TrueType. |
| recursive | Boolean | Se true, le cartelle specificate saranno scansionate ricorsivamente. |

## Esempi

Mostra come impostare una cartella di font personalizzata.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

// I file di font TrueType per tutti i font utilizzati nel progetto aperto dovrebbero trovarsi nella cartella MyFonts.
options.FontSettings.SetFontFolders(new string[] { "c:\\MyFonts"}, true);

project.Save(OutDir + "EstimatedMilestoneTasks_out4.pdf", options);
```

### Vedi anche

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


