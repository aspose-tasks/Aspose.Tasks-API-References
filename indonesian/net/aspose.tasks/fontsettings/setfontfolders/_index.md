---
title: "FontSettings.SetFontFolders"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode FontSettings. Menetapkan folder tempat Aspose.Tasks mencari font TrueType saat merender tampilan proyek"
type: docs
weight: 50
url: /id/net/aspose.tasks/fontsettings/setfontfolders/
---
## FontSettings.SetFontFolders method

Mengatur folder tempat Aspose.Tasks mencari font TrueType saat merender tampilan proyek.

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fontFolders | String[] | Array folder yang berisi font TrueType. |
| recursive | Boolean | Jika true, folder yang ditentukan akan dipindai secara rekursif. |

## Contoh

Menampilkan cara mengatur folder font khusus.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

// File font TrueType untuk semua font yang digunakan dalam proyek yang dibuka harus berada di folder MyFonts.
options.FontSettings.SetFontFolders(new string[] { "c:\\MyFonts"}, true);

project.Save(OutDir + "EstimatedMilestoneTasks_out4.pdf", options);
```

### Lihat Juga

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


