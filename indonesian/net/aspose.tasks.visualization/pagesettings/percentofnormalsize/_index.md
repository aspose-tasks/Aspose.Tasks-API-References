---
title: "PageSettings.PercentOfNormalSize"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PageSettings. Mendapatkan atau mengatur persentase ukuran normal untuk menyesuaikan pencetakan."
type: docs
weight: 90
url: /id/net/aspose.tasks.visualization/pagesettings/percentofnormalsize/
---
## PageSettings.PercentOfNormalSize property

Mendapatkan atau mengatur persentase ukuran normal untuk menyesuaikan pencetakan.

```csharp
public int PercentOfNormalSize { get; set; }
```

## Contoh

Menampilkan cara merender tampilan dengan faktor skala yang ditentukan.

```csharp
var project = new Project(DataDir + "Input.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);

// mengatur nilai yang menunjukkan bahwa tampilan harus diskalakan menggunakan faktor skala yang ditentukan
view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = true;
// tentukan faktor skala
view.PageInfo.PageSettings.PercentOfNormalSize = 33;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "PrintViewWithSpecifiedScaleFactor_out.pdf", saveOptions);
```

### Lihat Juga

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


