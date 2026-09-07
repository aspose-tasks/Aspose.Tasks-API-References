---
title: "Duration.GetHashCode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Duration. Mengembalikan nilai kode hash untuk objek ini"
type: docs
weight: 90
url: /id/net/aspose.tasks/duration/gethashcode/
---
## Duration.GetHashCode method

Mengembalikan nilai kode hash untuk objek ini.

```csharp
public override int GetHashCode()
```

### Nilai Kembali

mengembalikan nilai kode hash untuk instance durasi ini.

## Contoh

Menampilkan cara mendapatkan kode hash dari sebuah durasi.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// kode hash dari kalender didasarkan pada tipe satuan waktu dan nilai awal durasi
// sehingga kode hash berikutnya sama
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 2 Hash Code: {0}", duration2.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration2.GetHashCode()));

// tetapi kode hash dari durasi 1 dan 3 tidak sama
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 3 Hash Code: {0}", duration3.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration3.GetHashCode()));
```

### Lihat Juga

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


