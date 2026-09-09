---
title: "Filter.Criteria"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Filter özelliği. Görevlerin veya kaynakların MSP görünümünde görüntülenebilmesi için karşılaması gereken kriterleri alır veya ayarlar"
type: docs
weight: 20
url: /tr/net/aspose.tasks/filter/criteria/
---
## Filter.Criteria property

Görevlerin veya kaynakların MSP görünümünde görüntülenmesi için karşılaması gereken ölçütü alır veya ayarlar.

```csharp
public FilterCriteria Criteria { get; set; }
```

## Örnekler

Görev filtrelerinin nasıl okunacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine(filter.Criteria.CriteriaRows.Count);
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine(criteria1.Test.ToString());
Console.WriteLine(criteria1.Field.ToString());
Console.WriteLine(criteria1.Values[0].ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine(criteria21.Test.ToString());
Console.WriteLine(criteria21.Field.ToString());
Console.WriteLine(criteria21.Values[0].ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine(criteria22.Test.ToString());
Console.WriteLine(criteria22.Field.ToString());
Console.WriteLine(criteria22.Values[0].ToString());
Console.WriteLine(filter.Criteria);
```

### Ayrıca Bakınız

* class [FilterCriteria](../../filtercriteria/)
* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


