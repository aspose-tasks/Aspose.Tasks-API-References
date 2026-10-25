---
title: "Sınıf RateCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.RateCollection sınıfı. Rate nesnelerini içeren bir koleksiyonu temsil eder."
type: docs
weight: 1630
url: /tr/net/aspose.tasks/ratecollection/
---
## RateCollection class

[`Rate`](../rate/) nesnelerini içeren bir koleksiyonu temsil eder.

```csharp
public class RateCollection : IDictionary<RateType, RateByDateCollection>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/ratecollection/count/) { get; } | RateCollection içinde bulunan eleman sayısını alır. |
| [IsReadOnly](../../aspose.tasks/ratecollection/isreadonly/) { get; } | Bu koleksiyonun yalnızca okunabilir olup olmadığını gösteren bir değeri alır. |
| [Item](../../aspose.tasks/ratecollection/item/) { get; set; } | Belirtilen indeksteki öğeyi döndürür veya ayarlar. |
| [ParentResource](../../aspose.tasks/ratecollection/parentresource/) { get; } | Bu koleksiyon için ebeveyn [`Resource`](../resource/) nesnesini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/ratecollection/add/#add)(DateTime) | Bu koleksiyona yeni bir [`Rate`](../rate/) örneği ekler. |
| [Add](../../aspose.tasks/ratecollection/add/#add_1)(DateTime, RateType) | Bu koleksiyona yeni bir [`Rate`](../rate/) örneği ekler. |
| [GetEnumerator](../../aspose.tasks/ratecollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [Remove](../../aspose.tasks/ratecollection/remove/)(Rate) | Bu koleksiyondan Rate örneğini kaldırır. |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist)() | `RateCollection` nesnesini [`Rate`](../rate/) nesnelerinden oluşan bir listeye dönüştürür. |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist_1)(RateType) | `RateCollection` nesnesini belirtilen [`RateType`](../ratetype/) türüne göre filtrelenmiş [`Rate`](../rate/) nesnelerinden oluşan bir listeye dönüştürür. |

## Örnekler

Rate koleksiyonlarıyla nasıl çalışılacağını gösterir.

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

// İndeks erişimiyle en son oranı al.
var rateToUpdate = resource.Rates[RateType.B][new DateTime(2019, 11, 12, 8, 0, 0)];
rateToUpdate.RatesTo = new DateTime(2020, 12, 31, 17, 0, 0);
Console.WriteLine("Rates From: " + rateToUpdate.RatesFrom);
Console.WriteLine("Rates To: " + rateToUpdate.RatesTo);

// ...
// Oranlarla çalış.
// ...

// A türündeki tüm oranları kaldır.
List<Rate> rates = resource.Rates.ToList(RateType.A);
for (var i = 0; i < rates.Count; i++)
{
    var rateToRemove = rates[i];
    resource.Rates.Remove(rateToRemove);
}

// Rate koleksiyonunu düz bir listeye dönüştür.
Console.WriteLine("Iterate over the rates after remove the A-typed values: ");
List<Rate> list = resource.Rates.ToList();
foreach (var rt in list)
{
    Console.WriteLine("Rates From: " + rt.RatesFrom);
    Console.WriteLine("Rates To: " + rt.RatesTo);
    Console.WriteLine("Rate Table: " + rt.RateTable);
}
```

### Ayrıca Bakınız

* enum [RateType](../ratetype/)
* class [RateByDateCollection](../ratebydatecollection/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


