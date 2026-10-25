---
title: "Class RateCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.RateCollection. Mewakili koleksi yang berisi objek Rate"
type: docs
weight: 1630
url: /id/net/aspose.tasks/ratecollection/
---
## RateCollection class

Mewakili koleksi yang berisi objek [`Rate`](../rate/).

```csharp
public class RateCollection : IDictionary<RateType, RateByDateCollection>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/ratecollection/count/) { get; } | Mendapatkan jumlah elemen yang terdapat dalam RateCollection. |
| [IsReadOnly](../../aspose.tasks/ratecollection/isreadonly/) { get; } | Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca. |
| [Item](../../aspose.tasks/ratecollection/item/) { get; set; } | Mengembalikan atau mengatur elemen pada indeks yang ditentukan. |
| [ParentResource](../../aspose.tasks/ratecollection/parentresource/) { get; } | Mendapatkan objek induk [`Resource`](../resource/) untuk koleksi ini. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/ratecollection/add/#add)(DateTime) | Menambahkan instance [`Rate`](../rate/) baru ke koleksi ini. |
| [Add](../../aspose.tasks/ratecollection/add/#add_1)(DateTime, RateType) | Menambahkan instance [`Rate`](../rate/) baru ke koleksi ini. |
| [GetEnumerator](../../aspose.tasks/ratecollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [Remove](../../aspose.tasks/ratecollection/remove/)(Rate) | Menghapus instance Rate dari koleksi ini. |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist)() | Mengonversi objek `RateCollection` menjadi daftar objek [`Rate`](../rate/). |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist_1)(RateType) | Mengonversi objek `RateCollection` menjadi daftar objek [`Rate`](../rate/) yang difilter oleh tipe [`RateType`](../ratetype/) yang ditentukan. |

## Contoh

Menampilkan cara bekerja dengan koleksi tarif.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Test Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0), RateType.B);
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;

Console.WriteLine("Print rates of '{0}' resource: ", resource.Rates.ParentResource.Get(Rsc.Name));
Console.WriteLine("Count of rates: {0}", resource.Rates.Count);
Console.WriteLine("Is rate collection read-only: {0}", resource.Rates.IsReadOnly);
foreach (KeyValuePair<RateType, RateByDateCollection> sortedRates in resource.Rates)
{
    foreach (KeyValuePair<DateTime, Rate> pair in sortedRates.Value)
    {
        var rate = pair.Value;
        Console.WriteLine("Rates From: " + rate.RatesFrom);
        Console.WriteLine("Rates To: " + rate.RatesTo);
        Console.WriteLine("Rate Table: " + rate.RateTable);
        Console.WriteLine();
    }
}

// dapatkan tarif terbaru dengan akses indeks
var rateToUpdate = resource.Rates[RateType.B][new DateTime(2019, 11, 12, 8, 0, 0)];
rateToUpdate.RatesTo = new DateTime(2020, 12, 31, 17, 0, 0);
Console.WriteLine("Rates From: " + rateToUpdate.RatesFrom);
Console.WriteLine("Rates To: " + rateToUpdate.RatesTo);

// ...
// bekerja dengan tarif
// ...

// hapus semua tarif tipe A
List<Rate> rates = resource.Rates.ToList(RateType.A);
for (var i = 0; i < rates.Count; i++)
{
    var rateToRemove = rates[i];
    resource.Rates.Remove(rateToRemove);
}

// ubah koleksi tarif menjadi daftar datar
Console.WriteLine("Iterate over the rates after remove the A-typed values: ");
List<Rate> list = resource.Rates.ToList();
foreach (var rt in list)
{
    Console.WriteLine("Rates From: " + rt.RatesFrom);
    Console.WriteLine("Rates To: " + rt.RatesTo);
    Console.WriteLine("Rate Table: " + rt.RateTable);
}
```

### Lihat Juga

* enum [RateType](../ratetype/)
* class [RateByDateCollection](../ratebydatecollection/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


