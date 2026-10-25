---
title: "FontSettings.SetFontFolders"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "FontSettings‑Methode. Legt die Ordner fest, in denen Aspose.Tasks nach TrueType‑Schriften sucht, wenn die Projektansicht gerendert wird."
type: docs
weight: 50
url: /de/net/aspose.tasks/fontsettings/setfontfolders/
---
## FontSettings.SetFontFolders method

Legt die Ordner fest, in denen Aspose.Tasks nach TrueType‑Schriften sucht, wenn die Projektansicht gerendert wird.

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontFolders | String[] | Ein Array von Ordnern, die TrueType-Schriften enthalten. |
| rekursiv | Boolean | Wenn true, werden die angegebenen Ordner rekursiv durchsucht. |

## Beispiele

Zeigt, wie man einen benutzerdefinierten Schriftartenordner festlegt.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

// TrueType-Schriftdateien für alle im geöffneten Projekt verwendeten Schriften sollten im Ordner MyFonts liegen.
options.FontSettings.SetFontFolders(new string[] { "c:\\MyFonts"}, true);

project.Save(OutDir + "EstimatedMilestoneTasks_out4.pdf", options);
```

### Siehe auch

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


