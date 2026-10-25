---
title: "Rsc.AvailableTo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Tanggal akhir ketika sebuah sumber daya tersedia untuk bekerja pada unit yang ditentukan untuk periode waktu saat ini"
type: docs
weight: 130
url: /id/net/aspose.tasks/rsc/availableto/
---
## Rsc.AvailableTo field

Tanggal akhir ketika sumber daya tersedia untuk bekerja pada unit yang ditentukan untuk periode waktu saat ini.

```csharp
public static readonly Key<DateTime, RscKey> AvailableTo;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.AvailableTo.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableTo, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available To: " + resource.Get(Rsc.AvailableTo));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


