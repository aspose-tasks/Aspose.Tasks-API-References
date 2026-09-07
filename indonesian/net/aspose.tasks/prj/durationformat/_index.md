---
title: "Prj.DurationFormat"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Format untuk mengekspresikan durasi keseluruhan"
type: docs
weight: 300
url: /id/net/aspose.tasks/prj/durationformat/
---
## Prj.DurationFormat field

Format untuk menyatakan durasi total.

```csharp
public static readonly Key<TimeUnitType, PrjKey> DurationFormat;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.DurationFormat.

```csharp
var project = new Project();

project.Set(Prj.DurationFormat, TimeUnitType.Day);

Console.WriteLine("Duration Format: " + project.Get(Prj.DurationFormat));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


