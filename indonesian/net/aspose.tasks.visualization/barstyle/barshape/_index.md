---
title: "BarStyle.BarShape"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti BarStyle. Mendapatkan atau mengatur BarShape dari gaya bar"
type: docs
weight: 30
url: /id/net/aspose.tasks.visualization/barstyle/barshape/
---
## BarStyle.BarShape property

Mendapatkan atau mengatur `BarShape` dari gaya bar.

```csharp
public BarShape BarShape { get; set; }
```

## Contoh

Menampilkan cara menggunakan gaya batang khusus.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    BarStyles = new List<BarStyle>()
};

// tambahkan gaya batang untuk tugas tonggak.
var style = new BarStyle();
// atur <see cref="T:Aspose.Tasks.Visualization.BarItemType" /> dari gaya batang
style.ItemType = BarItemType.Milestone;
// atur <see cref="T:System.Drawing.Color" /> dari gaya batang.
style.BarColor = Color.Green;
// atur <see cref="P:Aspose.Tasks.Visualization.BarStyle.BarShape" /> dari gaya batang
style.BarShape = BarShape.HalfHeight;
// atur <see cref=\"T:Aspose.Tasks.Visualization.Shape\" /> di awal batang
style.StartShape = Shape.LeftBracket;
// atur <see cref=\"T:System.Drawing.Color\" /> dari bentuk di awal batang
style.StartShapeColor = Color.Aqua;
// atur <see cref=\"T:Aspose.Tasks.Visualization.Shape\" /> di akhir batang
style.EndShape = Shape.RightBracket;
// atur <see cref=\"T:System.Drawing.Color\" /> dari bentuk di akhir batang
style.EndShapeColor = Color.Aquamarine;
// atur teks yang akan dirender di kanan batang.
style.TextStyle = new TextStyle();
style.TextStyle.BackgroundColor = Color.Black;

// Ada fitur yang memungkinkan mengonversi teks batang.
// mari atur konverter untuk mendapatkan teks batang yang akan dirender.
style.LeftBarTextConverter = task =>
{
    if (!task.Get(Tsk.Name).StartsWith("T"))
    {
        task.Set(Tsk.Name, "T" + task.Get(Tsk.Name));
    }

    return task.Get(Tsk.Name);
};

options.BarStyles.Add(style);

// simpan proyek
project.Save(OutDir + "WorkWithBarStyle_out.mpp", options);
```

### Lihat Juga

* enum [BarShape](../../barshape/)
* class [BarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../barstyle/)
* assembly [Aspose.Tasks](../../../)


