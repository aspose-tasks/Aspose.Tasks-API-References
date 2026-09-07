---
title: "Kelas TableTextStyle"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Visualization.TableTextStyle. Mewakili gaya teks dalam tabel tampilan"
type: docs
weight: 3370
url: /id/net/aspose.tasks.visualization/tabletextstyle/
---
## TableTextStyle class

Mewakili gaya teks dalam tabel tampilan.

```csharp
public class TableTextStyle : TextStyle
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [TableTextStyle](tabletextstyle/#constructor)(int) | Menginisialisasi instance baru dari kelas `TableTextStyle`. |
| [TableTextStyle](tabletextstyle/#constructor_1)(int, FontDescriptor) | Menginisialisasi instance baru dari kelas `TableTextStyle` dengan font yang ditentukan. |
| [TableTextStyle](tabletextstyle/#constructor_2)(int, FontStyles) | Menginisialisasi instance baru dari kelas `TableTextStyle` dengan pengaturan font default dan gaya font yang ditentukan. |
| [TableTextStyle](tabletextstyle/#constructor_3)(int, float, FontStyles) | Menginisialisasi instance baru dari kelas `TableTextStyle` dengan ukuran font dan gaya font yang ditentukan. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | Mendapatkan atau mengatur warna latar belakang gaya teks. [`Color`](../textstyle/color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | Mendapatkan atau mengatur pola latar belakang gaya teks. [`BackgroundPattern`](../textstyle/backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | Mendapatkan atau mengatur warna teks. |
| [Field](../../aspose.tasks.visualization/tabletextstyle/field/) { get; set; } | Mendapatkan atau mengatur bidang yang akan diterapkan gaya. [`Field`](./field/). |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | Mendapatkan atau mengatur font gaya teks. |
| override [ItemType](../../aspose.tasks.visualization/tabletextstyle/itemtype/) { get; } | Mengembalikan nilai dari enum [`TextItemType`](../textitemtype/). |
| [RowUid](../../aspose.tasks.visualization/tabletextstyle/rowuid/) { get; } | Mendapatkan ID unik baris. Kembalikan -1 jika gaya diterapkan pada semua baris dalam tampilan. |

## Contoh

Menampilkan cara menyesuaikan gaya teks tabel yang digunakan untuk memberi gaya pada berbagai item teks dalam sebuah proyek.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// atur gaya teks nama tugas pertama
var style1 = new TableTextStyle(1);
// atur bidang yang akan diterapkan gaya.
style1.Field = Field.TaskName;
// atur <see cref=\"P:Aspose.Tasks.Visualization.TextStyle.Font\" /> dari gaya teks.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// atur ukuran dalam poin dari font gaya teks.

// atur gaya teks durasi tugas kedua
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // atur bendera yang menunjukkan bahwa data tampilan harus ditulis
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### Lihat Juga

* class [TextStyle](../textstyle/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


