---
title: "PageSettings.PagesInWidth"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PageSettings. Mendapatkan atau mengatur jumlah halaman dalam lebar yang akan dicetak."
type: docs
weight: 60
url: /id/net/aspose.tasks.visualization/pagesettings/pagesinwidth/
---
## PageSettings.PagesInWidth property

Mendapatkan atau mengatur jumlah halaman dalam lebar yang akan dicetak.

```csharp
public int PagesInWidth { get; set; }
```

## Contoh

Menampilkan cara merender tampilan dengan opsi 'Fit X to Y pages'.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.TaskUsage);

view.PageInfo.PageSettings.AdjustToPercentOfNormalSize = false;
// tentukan bahwa tampilan harus dirender dalam 2 halaman atau kurang dalam tinggi
view.PageInfo.PageSettings.PagesInHeight = 2;
// tentukan bahwa tampilan harus dirender dalam 1 halaman dalam lebar
view.PageInfo.PageSettings.PagesInWidth = 1;

PdfSaveOptions saveOptions = new PdfSaveOptions()
{
    ViewSettings = view,
    Timescale = Timescale.DefinedInView,
    StartDate =  new DateTime(2000, 04, 1),
    EndDate = new DateTime(2000, 12, 31)
};

project.Save(OutDir + "PrintViewWithFitToPages_out.pdf", saveOptions);
```

### Lihat Juga

* class [PageSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pagesettings/)
* assembly [Aspose.Tasks](../../../)


