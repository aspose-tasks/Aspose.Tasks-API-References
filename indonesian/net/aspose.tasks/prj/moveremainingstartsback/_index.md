---
title: "Prj.MoveRemainingStartsBack"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Menentukan apakah awal bagian sisa tugas yang dijadwalkan mulai setelah tanggal status namun dimulai lebih awal harus dipindahkan kembali ke tanggal status"
type: docs
weight: 510
url: /id/net/aspose.tasks/prj/moveremainingstartsback/
---
## Prj.MoveRemainingStartsBack field

Menentukan apakah awal bagian yang tersisa dari tugas yang dijadwalkan untuk mulai setelah tanggal status tetapi dimulai lebih awal harus dipindahkan kembali ke tanggal status.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsBack;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.MoveRemainingStartsBack.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsBack, true);

Console.WriteLine("Move Remaining Starts Back: " + project.Get(Prj.MoveRemainingStartsBack));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


