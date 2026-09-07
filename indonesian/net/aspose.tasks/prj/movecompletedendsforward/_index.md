---
title: "Prj.MoveCompletedEndsForward"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Menentukan apakah akhir bagian tugas yang selesai yang dijadwalkan selesai sebelum tanggal status tetapi dimulai kemudian harus dipindahkan ke tanggal status"
type: docs
weight: 500
url: /id/net/aspose.tasks/prj/movecompletedendsforward/
---
## Prj.MoveCompletedEndsForward field

Menentukan apakah akhir bagian tugas yang selesai yang dijadwalkan selesai sebelum tanggal status namun dimulai kemudian harus dipindahkan maju ke tanggal status.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsForward;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.MoveCompletedEndsForward.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsForward, true);

Console.WriteLine("Move Completed Ends Forward: " + project.Get(Prj.MoveCompletedEndsForward));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


