---
title: "MPPSaveOptions.ClearVba"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti MPPSaveOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah data makro VBA yang ada harus dihapus saat menyimpan proyek ke format MPP."
type: docs
weight: 20
url: /id/net/aspose.tasks.saving/mppsaveoptions/clearvba/
---
## MPPSaveOptions.ClearVba property

Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menghapus data makro VBA yang ada saat menyimpan proyek ke format MPP.

```csharp
public bool ClearVba { get; set; }
```

## Contoh

Menampilkan cara menghapus makro VBA dari file MPP.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

### Lihat Juga

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


