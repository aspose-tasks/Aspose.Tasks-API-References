---
title: "Enum Shape"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.Visualization.Shape enum. Bentuk penanda di awal atau akhir gaya batang yang akan dirender saat menyimpan data tampilan ke beberapa SaveFileFormat"
type: docs
weight: 3360
url: /id/net/aspose.tasks.visualization/shape/
---
## Shape enumeration

Bentuk penanda di awal atau akhir gaya batang yang akan dirender saat menyimpan data tampilan ke beberapa [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/).

```csharp
public enum Shape
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| None | `0` | Menunjukkan bentuk None. |
| VerticalLine | `1` | Menunjukkan bentuk garis vertikal. |
| Pentagon | `2` | Menunjukkan bentuk Pentagon. |
| Triangle | `3` | Menunjukkan bentuk Triangle. |
| LeftBracket | `4` | Menunjukkan bentuk kurung kiri. |
| RightBracket | `5` | Menunjukkan bentuk kurung kanan. |
| ArrowDown | `6` | Menunjukkan bentuk ArrowDown. |
| LeftFade | `7` | Menunjukkan bentuk fade kiri. |
| RightFade | `8` | Menunjukkan bentuk fade kanan. |
| Diamond | `9` | Menunjukkan bentuk Diamond. |
| Circle | `10` | Menunjukkan bentuk Circle. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


