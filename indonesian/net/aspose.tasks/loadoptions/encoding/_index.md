---
title: "LoadOptions.Encoding"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti LoadOptions. Mendapatkan atau mengatur encoding yang digunakan untuk membaca proyek dari format HTML, MPX, XER, dan Primavera XML. Encoding default adalah UTF8."
type: docs
weight: 30
url: /id/net/aspose.tasks/loadoptions/encoding/
---
## LoadOptions.Encoding property

Mendapatkan atau mengatur encoding yang digunakan untuk membaca proyek dari format HTML, MPX, XER, dan Primavera XML. Encoding default adalah UTF8.

```csharp
public Encoding Encoding { get; set; }
```

## Contoh

Menampilkan cara menentukan encoding saat membuka proyek dari file Primavera XER.

```csharp
LoadOptions lo = new LoadOptions();
lo.Encoding = Encoding.GetEncoding(1251);
lo.PrimaveraReadOptions = new PrimaveraReadOptions();
var project = new Project("encoding1251.xer", lo);
```

### Lihat Juga

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


