---
title: "Project.DefaultView"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Project. Mendapatkan atau mengatur tampilan default proyek"
type: docs
weight: 360
url: /id/net/aspose.tasks/project/defaultview/
---
## Project.DefaultView property

Mendapatkan atau mengatur tampilan default proyek.

```csharp
public View DefaultView { get; set; }
```

## Contoh

Menampilkan cara bekerja dengan tampilan default proyek.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// Dapatkan tampilan default
UsageView view = (TaskUsageView)project.DefaultView;

// Kolom header detail tidak akan ditampilkan
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// Tampilkan kolom header detail
view.DisplayDetailsHeaderColumn = true;

// Ulangi header detail pada semua baris penugasan
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

Menampilkan cara bekerja dengan tampilan Project dan menambahkan kolom ke tampilan default (yang ditampilkan ketika file MPP dibuka di MS Project).

```csharp
// buat proyek kosong tanpa tampilan
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// Modifikasi tampilan default (ini adalah tampilan diagram Gantt).
// Atau Anda dapat memilih tampilan berdasarkan nama atau melalui Layar Tampilan menggunakan koleksi project.View.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// Flag WriteViewData harus digunakan untuk menyimpan perubahan properti tampilan.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

### Lihat Juga

* class [View](../../view/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


