---
title: "MPPSaveOptions.RemoveInvalidAssignments"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti MPPSaveOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah penugasan sumber daya yang tidak valid harus dihapus saat menyimpan ke MPP. MS Project membuat penugasan sumber daya kosong untuk setiap tugas. Atur flag ini ke true untuk menghapusnya saat menyimpan."
type: docs
weight: 40
url: /id/net/aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/
---
## MPPSaveOptions.RemoveInvalidAssignments property

Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menghapus penugasan sumber daya yang tidak valid saat menyimpan ke MPP. MS Project membuat penugasan sumber daya kosong untuk setiap tugas. Atur flag ini ke true untuk menghapusnya saat menyimpan.

```csharp
public bool RemoveInvalidAssignments { get; set; }
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


