---
title: "TableTextStyle.ItemType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti TableTextStyle. Mengembalikan nilai dari enum TextItemType."
type: docs
weight: 30
url: /id/net/aspose.tasks.visualization/tabletextstyle/itemtype/
---
## TableTextStyle.ItemType property

Mengembalikan nilai dari enum [`TextItemType`](../../textitemtype/).

```csharp
public override TextItemType ItemType { get; }
```

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

* enum [TextItemType](../../textitemtype/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


