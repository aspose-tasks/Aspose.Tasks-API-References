---
title: "LoadOptions.CancellationToken"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti LoadOptions. Mendapatkan atau mengatur token yang dapat digunakan untuk membatalkan operasi pemuatan proyek."
type: docs
weight: 20
url: /id/net/aspose.tasks/loadoptions/cancellationtoken/
---
## LoadOptions.CancellationToken property

Mendapatkan atau mengatur token yang dapat digunakan untuk membatalkan operasi pemuatan proyek.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Contoh

Menampilkan cara melewatkan CancellationToken untuk membatalkan operasi pemuatan Proyek yang berjalan lama.

```csharp
var loadOptions = new LoadOptions();

CancellationTokenSource cts = new CancellationTokenSource();
loadOptions.CancellationToken = cts.Token;

// cts dapat diteruskan ke thread lain dimana metode cts.Cancel() dapat dipanggil untuk membatalkan operasi pemuatan proyek.
// cts.Cancel();
var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
```

### Lihat Juga

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


