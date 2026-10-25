---
title: "Rsc.StandardRateFormat"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Unit yang digunakan oleh Microsoft Project untuk menampilkan tarif standar"
type: docs
weight: 630
url: /id/net/aspose.tasks/rsc/standardrateformat/
---
## Rsc.StandardRateFormat field

Unit yang digunakan oleh Microsoft Project untuk menampilkan tarif standar.

```csharp
public static readonly Key<RateFormatType, RscKey> StandardRateFormat;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.StandardRateFormat.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


