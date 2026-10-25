---
title: "Filter.CompareTo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Filter. Membandingkan instance ini dengan instance yang ditentukan dari kelas Filter dan mengembalikan indikasi urutan relatif mereka"
type: docs
weight: 90
url: /id/net/aspose.tasks/filter/compareto/
---
## Filter.CompareTo method

Membandingkan instance ini dengan instance yang ditentukan dari kelas [`Filter`](../) dan mengembalikan indikasi urutan relatif mereka.

```csharp
public int CompareTo(Filter other)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | Filter | instance yang ditentukan dari kelas [`Filter`](../) untuk dibandingkan dengan objek ini. |

### Nilai Kembali

indikasi urutan relatif mereka.

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


