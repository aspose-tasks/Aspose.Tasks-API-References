---
title: "Filter.op_Inequality"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Filter. Mengembalikan nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan."
type: docs
weight: 150
url: /id/net/aspose.tasks/filter/op_inequality/
---
## Filter Inequality operator

Kembalikan nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan.

```csharp
public static bool operator !=(Filter a, Filter b)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| a | Filter | Filter pertama. |
| b | Filter | Filter kedua. |

### Nilai Kembali

nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan

## Contoh

Menampilkan cara memeriksa kesetaraan filter.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();

var filter1 = filters[0];
var filter2 = filters[1];

// kesetaraan filter diperiksa terhadap UID filter.
Console.WriteLine("Filter 1 UID: " + filter1.Uid);
Console.WriteLine("Filter 2 UID: " + filter2.Uid);
Console.WriteLine("Are filters equal: " + filter1.Equals(filter2));
```

### Lihat Juga

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


