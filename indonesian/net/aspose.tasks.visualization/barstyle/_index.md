---
title: "Class BarStyle"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Visualization.BarStyle. Mengubah gaya visual bar untuk item dalam tampilan proyek."
type: docs
weight: 2960
url: /id/net/aspose.tasks.visualization/barstyle/
---
## BarStyle class

Ubah gaya visual batang untuk item dalam tampilan proyek.

```csharp
public class BarStyle
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [BarStyle](barstyle/)() | Menginisialisasi instance baru dari kelas `BarStyle`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [BarColor](../../aspose.tasks.visualization/barstyle/barcolor/) { get; set; } | Mendapatkan atau mengatur Warna dari gaya bar. |
| [BarShape](../../aspose.tasks.visualization/barstyle/barshape/) { get; set; } | Mendapatkan atau mengatur [`BarShape`](./barshape/) dari gaya bar. |
| [BottomBarTextConverter](../../aspose.tasks.visualization/barstyle/bottombartextconverter/) { get; set; } | Mendapatkan atau mengatur konverter yang ditentukan pengguna untuk mendapatkan teks yang akan ditampilkan di bagian bawah batang tugas. Menimpa nilai properti [`BottomField`](./bottomfield/). |
| [BottomField](../../aspose.tasks.visualization/barstyle/bottomfield/) { get; set; } | Mendapatkan atau mengatur bidang yang akan ditampilkan di bagian bawah bar. |
| [EndShape](../../aspose.tasks.visualization/barstyle/endshape/) { get; set; } | Mendapatkan atau mengatur [`Shape`](../shape/) di akhir bar. |
| [EndShapeColor](../../aspose.tasks.visualization/barstyle/endshapecolor/) { get; set; } | Mendapatkan atau mengatur Warna dari bentuk di akhir bar. |
| [EndShapeType](../../aspose.tasks.visualization/barstyle/endshapetype/) { get; set; } | Mendapatkan atau mengatur tipe bentuk akhir. [`GanttBarType`](../ganttbartype/). |
| [From](../../aspose.tasks.visualization/barstyle/from/) { get; set; } | Mendapatkan atau mengatur posisi titik awal batang gantt. [`Field`](../../aspose.tasks/field/). |
| [InsideBarTextConverter](../../aspose.tasks.visualization/barstyle/insidebartextconverter/) { get; set; } | Mendapatkan atau mengatur konverter yang ditentukan pengguna untuk mendapatkan teks yang akan ditampilkan di dalam batang tugas. Menimpa nilai properti [`InsideField`](./insidefield/). |
| [InsideField](../../aspose.tasks.visualization/barstyle/insidefield/) { get; set; } | Mendapatkan atau mengatur bidang yang akan ditampilkan di dalam bar. |
| [ItemType](../../aspose.tasks.visualization/barstyle/itemtype/) { get; set; } | Mendapatkan atau mengatur [`BarItemType`](../baritemtype/) dari gaya bar. |
| [LeftBarTextConverter](../../aspose.tasks.visualization/barstyle/leftbartextconverter/) { get; set; } | Mendapatkan atau mengatur konverter yang didefinisikan pengguna untuk mendapatkan teks yang akan ditampilkan di sebelah kiri bar tugas. Menimpa nilai properti [`LeftField`](./leftfield/). |
| [LeftField](../../aspose.tasks.visualization/barstyle/leftfield/) { get; set; } | Mendapatkan atau mengatur bidang yang akan ditampilkan di sebelah kiri bar. |
| [RightBarTextConverter](../../aspose.tasks.visualization/barstyle/rightbartextconverter/) { get; set; } | Mendapatkan atau mengatur konverter yang ditentukan pengguna untuk mendapatkan teks yang akan ditampilkan di sebelah kanan batang tugas. Menimpa nilai properti [`RightField`](./rightfield/). |
| [RightField](../../aspose.tasks.visualization/barstyle/rightfield/) { get; set; } | Mendapatkan atau mengatur bidang yang akan ditampilkan di sebelah kanan batang. |
| [StartShape](../../aspose.tasks.visualization/barstyle/startshape/) { get; set; } | Mendapatkan atau mengatur [`Shape`](../shape/) di awal batang. |
| [StartShapeColor](../../aspose.tasks.visualization/barstyle/startshapecolor/) { get; set; } | Mendapatkan atau mengatur Warna bentuk di awal batang. |
| [StartShapeType](../../aspose.tasks.visualization/barstyle/startshapetype/) { get; set; } | Mendapatkan atau mengatur tipe bentuk awal. |
| [TextStyle](../../aspose.tasks.visualization/barstyle/textstyle/) { get; set; } | Mendapatkan atau mengatur gaya teks batang. |
| [To](../../aspose.tasks.visualization/barstyle/to/) { get; set; } | Mendapatkan atau mengatur posisi titik akhir batang gantt. |
| [TopBarTextConverter](../../aspose.tasks.visualization/barstyle/topbartextconverter/) { get; set; } | Mendapatkan atau mengatur konverter yang ditentukan pengguna untuk mendapatkan teks yang akan dirender di bagian atas batang tugas. Menimpa nilai properti [`TopField`](./topfield/). |
| [TopField](../../aspose.tasks.visualization/barstyle/topfield/) { get; set; } | Mendapatkan atau mengatur bidang yang akan ditampilkan di bagian atas batang. |

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


