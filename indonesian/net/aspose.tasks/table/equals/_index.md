---
title: "Table.Equals"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Table. Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan"
type: docs
weight: 120
url: /id/net/aspose.tasks/table/equals/
---
## Table.Equals method

Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

```csharp
public override bool Equals(object obj)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | Objek | Objek untuk dibandingkan dengan instance ini. |

### Nilai Kembali

**True** if the specified object is a Table that has the same UID value as this instance; otherwise, **false**.

## Contoh

Menampilkan cara memeriksa kesetaraan tabel.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// Kesetaraan tabel diperiksa terhadap UID tabel.
Console.WriteLine("Table 1 UID: " + table1.Uid);
Console.WriteLine("Table 2 UID: " + table2.Uid);
Console.WriteLine("Are tables equal: " + table1.Equals(table2));
```

### Lihat Juga

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


