---
title: "Prj.MoveCompletedEndsBack"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Menentukan apakah akhir bagian tugas yang selesai, yang dijadwalkan mulai setelah tanggal status namun dimulai lebih awal, harus dipindahkan kembali ke tanggal status"
type: docs
weight: 490
url: /id/net/aspose.tasks/prj/movecompletedendsback/
---
## Prj.MoveCompletedEndsBack field

Menentukan apakah akhir bagian tugas yang selesai yang dijadwalkan mulai setelah tanggal status namun dimulai lebih awal harus dipindahkan kembali ke tanggal status.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsBack;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.MoveCompletedEndsBack.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsBack, true);

Console.WriteLine("Move Completed Ends Back: " + project.Get(Prj.MoveCompletedEndsBack));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


