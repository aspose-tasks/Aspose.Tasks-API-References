---
title: "Sınıf FilterCriteria"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.FilterCriteria sınıfı. Görevlerin veya kaynakların MSP görünümünde görüntülenmesi için karşılaması gereken ölçütleri tanımlar."
type: docs
weight: 630
url: /tr/net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

Görevlerin veya kaynakların MSP görünümünde görüntülenmesi için karşılaması gereken kriterleri tanımlar.

```csharp
public class FilterCriteria
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | Alt `FilterCriteria` satırlarının listesini alır. Filtre birden fazla ölçüt satırı içeriyorsa, And operatörünün etkisi, görevin veya kaynağın bu filtrenin sonucu olarak görüntülenmesi için her iki satırın da ölçütlerini karşılaması gerektiğidir. Or operatörünün etkisi ise bir satırın ölçütünün karşılanması gerektiğidir. |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | `[`Field`](./field/)` öğesini alır veya ayarlar. |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | FieldName, Test ve Value ile oluşturulan ölçütü alır veya ayarlar; bu ölçüt filtre içindeki diğer ölçütlerle ilişkilidir. |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | FieldName ve Value arasında yapılan karşılaştırma türünü alır veya ayarlar; bu, filtre için seçim ölçütü olarak kullanılır. [`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | FieldName ile belirtilen alanın değeriyle karşılaştırılacak nesne değerlerini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [IsFieldValue](../../aspose.tasks/filtercriteria/isfieldvalue/)() | FilterCriteria'nin sağ tarafındaki değerin sabit bir değer değil, bir alan referansı olup olmadığını alır. |
| [SetValueField](../../aspose.tasks/filtercriteria/setvaluefield/)(Field) | FieldName ile belirtilen alanın değeriyle karşılaştırılacak değere sahip alanı ayarlar. |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | `FilterCriteria` sınıfının örneğinin dize temsilini döndürür. |

## Örnekler

Görev filtre kriterlerini nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine("Count of criteria rows: " + filter.Criteria.CriteriaRows.Count);
foreach (var row in filter.Criteria.CriteriaRows)
{
    Console.WriteLine("Field: " + row.Field);
    Console.WriteLine("Operation: " + row.Operation);
    Console.WriteLine("Test: " + row.Test);

    var values = row.Values.Where(c => c != null).ToArray();
    if (values.Length == 0)
    {
        continue;
    }

    Console.WriteLine("Value{0}: {1}", values.Length == 1 ? "" : "s", string.Join(", ", values));
}

// filtre kriterlerini string olarak yazdır 
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine("Criteria filter 1:");
Console.WriteLine(criteria1.ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);
Console.WriteLine("Criteria filter 2:");
Console.WriteLine(criteria2.ToString());

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine("Criteria filter 21:");
Console.WriteLine(criteria21.ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine("Criteria filter 22:");
Console.WriteLine(criteria22.ToString());
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


