---
title: "Rsc.RemainingWork"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Waktu yang masih diperlukan untuk menyelesaikan sebuah tugas atau sekumpulan tugas"
type: docs
weight: 610
url: /id/net/aspose.tasks/rsc/remainingwork/
---
## Rsc.RemainingWork field

Waktu yang masih diperlukan untuk menyelesaikan sebuah tugas atau sekumpulan tugas.

```csharp
public static readonly Key<Duration, RscKey> RemainingWork;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.RemainingWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + resource.Get(Rsc.RemainingWork));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


