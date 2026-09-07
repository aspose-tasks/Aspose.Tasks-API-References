---
title: "Kelas Filter"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Filter. Mewakili sebuah filter dalam Project"
type: docs
weight: 600
url: /id/net/aspose.tasks/filter/
---
## Filter class

Mewakili filter dalam Project.

```csharp
public sealed class Filter : IComparable<Filter>, IEquatable<Filter>
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [Filter](filter/)() | Konstruktor default. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Criteria](../../aspose.tasks/filter/criteria/) { get; set; } | Mendapatkan atau mengatur kriteria yang harus dipenuhi tugas atau sumber daya untuk ditampilkan dalam tampilan MSP. |
| [FilterType](../../aspose.tasks/filter/filtertype/) { get; set; } | Mendapatkan tipe filter. |
| [Index](../../aspose.tasks/filter/index/) { get; } | Mendapatkan indeks dari objek `Filter` dalam objek yang berisi Filters. |
| [Name](../../aspose.tasks/filter/name/) { get; set; } | Mendapatkan atau mengatur nama objek Filter. |
| [ShowInMenu](../../aspose.tasks/filter/showinmenu/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah proyek menampilkan nama filter dalam daftar drop-down Filter pada tab View di Ribbon. |
| [ShowRelatedSummaryRows](../../aspose.tasks/filter/showrelatedsummaryrows/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah baris ringkasan terkait ditampilkan untuk filter. |
| [Uid](../../aspose.tasks/filter/uid/) { get; } | Mendapatkan pengidentifikasi unik dari filter. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [CompareTo](../../aspose.tasks/filter/compareto/)(Filter) | Bandingkan instance ini dengan instance yang ditentukan dari kelas `Filter` dan kembalikan indikasi urutan relatif mereka. |
| [Equals](../../aspose.tasks/filter/equals/#equals)(Filter) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek AssignmentBaseline yang ditentukan. |
| override [Equals](../../aspose.tasks/filter/equals/#equals_1)(object) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek AssignmentBaseline yang ditentukan. |
| override [GetHashCode](../../aspose.tasks/filter/gethashcode/)() | Kembalikan nilai kode hash untuk filter. |
| [operator ==](../../aspose.tasks/filter/op_equality/) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [operator &gt;](../../aspose.tasks/filter/op_greaterthan/) | Kembalikan nilai yang menunjukkan apakah instance ini lebih besar dari objek yang ditentukan. |
| [operator &gt;=](../../aspose.tasks/filter/op_greaterthanorequal/) | Kembalikan nilai yang menunjukkan apakah instance ini lebih besar atau sama dengan objek yang ditentukan. |
| [operator !=](../../aspose.tasks/filter/op_inequality/) | Kembalikan nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan. |
| [operator &lt;](../../aspose.tasks/filter/op_lessthan/) | Kembalikan nilai yang menunjukkan apakah instance ini lebih kecil dari objek yang ditentukan. |
| [operator &lt;=](../../aspose.tasks/filter/op_lessthanorequal/) | Kembalikan nilai yang menunjukkan apakah instance ini lebih kecil atau sama dengan objek yang ditentukan. |

## Contoh

Menampilkan cara bekerja dengan filter.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();
Console.WriteLine("Task filters count: " + filters.Count);
foreach (var filter in filters)
{
    Console.WriteLine("Uid: " + filter.Uid);
    Console.WriteLine("Index: " + filter.Index);
    Console.WriteLine("Name: " + filter.Name);
    Console.WriteLine("Type: " + filter.FilterType);
    Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
}

// periksa filter sumber daya
List<Filter> resourceFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + resourceFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + resourceFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + resourceFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + resourceFilters[0].ShowRelatedSummaryRows);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


