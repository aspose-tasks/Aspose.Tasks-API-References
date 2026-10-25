---
title: "Enum FilterComparisonType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.FilterComparisonType enum. FieldName ile Value arasında yapılan karşılaştırma türü, bir filtre veya grafik gösterge için seçim kriteri olarak işlev görür."
type: docs
weight: 620
url: /tr/net/aspose.tasks/filtercomparisontype/
---
## FilterComparisonType enumeration

Filtre veya grafik gösterge için seçim kriteri olarak işlev gören FieldName ve Value arasında yapılan karşılaştırma türü.

```csharp
public enum FilterComparisonType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Equals | `6` | Field değerinin Value'ye eşit olması. |
| DoesNotEqual | `7` | Field değerinin Value'ye eşit olmaması. |
| IsGreaterThan | `2` | Field değerinin Value'den büyük olması. |
| IsGreaterThanOrEqualTo | `4` | Field değerinin Value'ye eşit veya daha büyük olması. |
| IsLessThan | `3` | Field değerinin Value'den küçük olması. |
| IsLessThanOrEqualTo | `5` | Field değerinin Value'ye eşit veya daha küçük olması. |
| IsWithin | `1` | Field değerinin Value içinde olması. |
| IsNotWithin | `9` | Field değerinin Value içinde olmaması. |
| Contains | `8` | Field değerinin Value'yi içermesi. |
| DoesNotContain | `10` | Field değerinin Value'yi içermemesi. |
| ContainsExactly | `11` | Field değerinin Value'yi tam olarak içermesi. |
| IsOneOf | `12` | Field değerinin belirtilen Values değerlerinden birine eşit olması. AutoFilters içinde kullanılır. |
| Undefined | `0` | Tanımsız değer. |
| IsAnyValue | `255` | 'Is any value' koşulu. Grafik göstergeler için uygulanabilir. |

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


