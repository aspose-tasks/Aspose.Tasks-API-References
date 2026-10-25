---
title: "MPPSaveOptions.WriteViewData"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti MPPSaveOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah data tampilan harus ditulis saat menyimpan proyek ke format MPP. Data tampilan mencakup koleksi Project.Views Filters dan Tables."
type: docs
weight: 80
url: /id/net/aspose.tasks.saving/mppsaveoptions/writeviewdata/
---
## MPPSaveOptions.WriteViewData property

Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menulis data tampilan saat menyimpan proyek ke format MPP. Data tampilan mencakup koleksi Project.Views, Filters, dan Tables.

```csharp
public bool WriteViewData { get; set; }
```

## Contoh

Menampilkan cara menyimpan proyek ke dalam stream sebagai file MPP.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

    // buat opsi penyimpanan
    SimpleSaveOptions options = new MPPSaveOptions
    {
        // mengatur nilai yang menunjukkan apakah akan menghapus penugasan sumber daya tidak valid saat menyimpan ke MPP
        RemoveInvalidAssignments = true
    };

    // simpan MPP dengan opsi
    project.Save(stream, options);
}
```

### Lihat Juga

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


