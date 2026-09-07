---
title: "Filter.Equals"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Filter. Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek AssignmentBaseline yang ditentukan."
type: docs
weight: 100
url: /id/net/aspose.tasks/filter/equals/
---
## Equals(Filter) {#equals}

Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek AssignmentBaseline yang ditentukan.

```csharp
public bool Equals(Filter other)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| lain | Filter | objek AssignmentBaseline yang ditentukan untuk dibandingkan dengan instance ini. |

### Nilai Kembali

mengembalikan true jika instance ini sama dengan objek AssignmentBaseline yang ditentukan; jika tidak, false.

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

---

## Equals(object) {#equals_1}

Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek AssignmentBaseline yang ditentukan.

```csharp
public override bool Equals(object obj)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | Objek | objek AssignmentBaseline yang ditentukan untuk dibandingkan dengan instance ini. |

### Nilai Kembali

mengembalikan true jika instance ini sama dengan objek AssignmentBaseline yang ditentukan; jika tidak, false.

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


