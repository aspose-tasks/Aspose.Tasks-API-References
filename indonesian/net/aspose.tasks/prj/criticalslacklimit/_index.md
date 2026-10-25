---
title: "Prj.CriticalSlackLimit"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Tugas dianggap kritis oleh MS Project jika total slack kurang atau sama dengan jumlah hari ini"
type: docs
weight: 140
url: /id/net/aspose.tasks/prj/criticalslacklimit/
---
## Prj.CriticalSlackLimit field

Tugas dianggap kritis oleh MS Project jika total slack kurang atau sama dengan jumlah hari ini.

```csharp
public static readonly Key<int, PrjKey> CriticalSlackLimit;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.CriticalSlackLimit.

```csharp
var project = new Project();

project.Set(Prj.CriticalSlackLimit, 2);

Console.WriteLine("Critical Slack Limit: " + project.Get(Prj.CriticalSlackLimit));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


