---
title: "Prj.ActualsInSync"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Menentukan apakah semua pekerjaan aktual telah disinkronkan dengan proyek"
type: docs
weight: 10
url: /id/net/aspose.tasks/prj/actualsinsync/
---
## Prj.ActualsInSync field

Menentukan apakah semua pekerjaan aktual telah disinkronkan dengan proyek.

```csharp
public static readonly Key<NullableBool, PrjKey> ActualsInSync;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.ActualsInSync.

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


