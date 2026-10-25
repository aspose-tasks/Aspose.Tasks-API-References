---
title: "PageSettings.AdjustToPercentOfNormalSize"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PageSettings. Mendapatkan atau mengatur nilai yang menunjukkan apakah pencetakan harus disesuaikan ke persentase PercentOfNormalSize dari ukuran normal yang ditentukan."
type: docs
weight: 20
url: /id/net/aspose.tasks.visualization/pagesettings/adjusttopercentofnormalsize/
---
## PageSettings.AdjustToPercentOfNormalSize property

Mendapatkan atau mengatur nilai yang menunjukkan apakah pencetakan harus disesuaikan ke persentase ([`PercentOfNormalSize`](../percentofnormalsize/)) dari ukuran normal.

```csharp
public bool AdjustToPercentOfNormalSize { get; set; }
```

## Catatan

Tidak efektif ketika proyek dirender dalam format HTML.

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


