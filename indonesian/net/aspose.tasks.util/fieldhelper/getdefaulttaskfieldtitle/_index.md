---
title: "FieldHelper.GetDefaultTaskFieldTitle"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode FieldHelper. Mengembalikan judul default dari field tugas tertentu"
type: docs
weight: 20
url: /id/net/aspose.tasks.util/fieldhelper/getdefaulttaskfieldtitle/
---
## FieldHelper.GetDefaultTaskFieldTitle method

Mengembalikan judul default dari bidang tugas spesifik.

```csharp
public static string GetDefaultTaskFieldTitle(TaskKey taskKey)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| taskKey | TaskKey | Field tugas untuk mendapatkan judul default. |

### Nilai Kembali

Judul default dari field tugas tertentu jika field tersebut dapat ditampilkan dalam tampilan MS Project, null jika tidak.

## Contoh

Menunjukkan cara mendapatkan judul default field untuk field tugas tertentu.

```csharp
Console.WriteLine("Title for Tsk.ActualCost: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.ActualCost.KeyType));
Console.WriteLine("Title for Tsk.PercentWorkComplete: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.PercentWorkComplete.KeyType));
```

### Lihat Juga

* enum [TaskKey](../../../aspose.tasks/taskkey/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


