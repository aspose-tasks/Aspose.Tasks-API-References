---
title: "Gridline.Equals"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Gridline. Mengembalikan flag yang menunjukkan apakah instance ini sama dengan objek yang ditentukan."
type: docs
weight: 50
url: /id/net/aspose.tasks.visualization/gridline/equals/
---
## Gridline.Equals method

Mengembalikan flag yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

```csharp
public override bool Equals(object obj)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | Objek | objek yang ditentukan untuk dibandingkan dengan instance ini. |

### Nilai Kembali

sebuah flag yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

## Contoh

Menampilkan cara memeriksa kesetaraan gridline.

```csharp
var gridline1 = new Gridline();
var gridline2 = new Gridline();

// kesetaraan gridline diperiksa terhadap tipe gridline.
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Gridline 2 Type: " + gridline2.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));

// ubah tipe
gridline1.GridlineType = GridlineType.BarRows;
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));
```

### Lihat Juga

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


