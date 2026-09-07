---
title: "Table.GetHashCode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Table. Mengembalikan kode hash untuk Table ini"
type: docs
weight: 130
url: /id/net/aspose.tasks/table/gethashcode/
---
## Table.GetHashCode method

Mengembalikan kode hash untuk Tabel ini.

```csharp
public override int GetHashCode()
```

### Nilai Kembali

Mengembalikan nilai kode hash untuk objek ini.

## Contoh

Menampilkan cara mendapatkan kode hash dari sebuah tabel.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

List<Table> tables = project.Tables.ToList();

var table1 = tables[0];
var table2 = tables[1];

// Kode hash sebuah tabel sama dengan UID tabel 
Console.WriteLine("Table UID: {0} Hash Code: {1}", table1.Uid, table1.GetHashCode());
Console.WriteLine("Table UID: {0} Hash Code: {1}", table2.Uid, table2.GetHashCode());
```

### Lihat Juga

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


