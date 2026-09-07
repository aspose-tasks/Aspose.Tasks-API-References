---
title: "NullableBool.GetHashCode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode NullableBool. Mengembalikan nilai kode hash untuk instance dari kelas NullableBool."
type: docs
weight: 50
url: /id/net/aspose.tasks/nullablebool/gethashcode/
---
## NullableBool.GetHashCode method

Mengembalikan nilai kode hash untuk instance dari kelas [`NullableBool`](../).

```csharp
public override int GetHashCode()
```

### Nilai Kembali

mengembalikan nilai kode hash untuk objek ini.

## Contoh

Menunjukkan cara bekerja dengan &lt;see cref=\"Aspose.Tasks.NullableBool\" /&gt;.GetHashCode method.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// kode hash dari bool didasarkan pada properti 'IsDefined' dan 'Value'
Console.WriteLine("Bool 1: {0} Hash Code 1: {1}", bool1.ToString(), bool1.GetHashCode());
Console.WriteLine("Bool 2: {0} Hash Code 1: {1}", bool2.ToString(), bool2.GetHashCode());
```

### Lihat Juga

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


