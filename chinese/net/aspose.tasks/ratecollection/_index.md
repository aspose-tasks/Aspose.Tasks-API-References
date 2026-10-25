---
title: "类 RateCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.RateCollection 类。表示包含 Rate 对象的集合"
type: docs
weight: 1630
url: /zh/net/aspose.tasks/ratecollection/
---
## RateCollection class

表示包含 [`Rate`](../rate/) 对象的集合。

```csharp
public class RateCollection : IDictionary<RateType, RateByDateCollection>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/ratecollection/count/) { get; } | 获取 RateCollection 中包含的元素数量。 |
| [IsReadOnly](../../aspose.tasks/ratecollection/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读。 |
| [Item](../../aspose.tasks/ratecollection/item/) { get; set; } | 返回或设置指定索引处的元素。 |
| [ParentResource](../../aspose.tasks/ratecollection/parentresource/) { get; } | 获取此集合的父级 [`Resource`](../resource/) 对象。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/ratecollection/add/#add)(DateTime) | 向此集合添加一个新的 [`Rate`](../rate/) 实例。 |
| [Add](../../aspose.tasks/ratecollection/add/#add_1)(DateTime, RateType) | 向此集合添加一个新的 [`Rate`](../rate/) 实例。 |
| [GetEnumerator](../../aspose.tasks/ratecollection/getenumerator/)() | 返回此集合的枚举器。 |
| [Remove](../../aspose.tasks/ratecollection/remove/)(Rate) | 从此集合中移除 Rate 实例。 |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist)() | `RateCollection` 对象转换为 [`Rate`](../rate/) 对象列表。 |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist_1)(RateType) | `RateCollection` 对象转换为按指定 [`RateType`](../ratetype/) 类型过滤的 [`Rate`](../rate/) 对象列表。 |

## 示例

展示如何使用费率集合。

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

// 通过索引访问获取最新费率
var rateToUpdate = resource.Rates[RateType.B][new DateTime(2019, 11, 12, 8, 0, 0)];
rateToUpdate.RatesTo = new DateTime(2020, 12, 31, 17, 0, 0);
Console.WriteLine("Rates From: " + rateToUpdate.RatesFrom);
Console.WriteLine("Rates To: " + rateToUpdate.RatesTo);

// ...
// 使用费率
// ...

// 移除所有类型为 A 的费率
List<Rate> rates = resource.Rates.ToList(RateType.A);
for (var i = 0; i < rates.Count; i++)
{
    var rateToRemove = rates[i];
    resource.Rates.Remove(rateToRemove);
}

// 将费率集合转换为平面列表
Console.WriteLine("Iterate over the rates after remove the A-typed values: ");
List<Rate> list = resource.Rates.ToList();
foreach (var rt in list)
{
    Console.WriteLine("Rates From: " + rt.RatesFrom);
    Console.WriteLine("Rates To: " + rt.RatesTo);
    Console.WriteLine("Rate Table: " + rt.RateTable);
}
```

### 另见

* enum [RateType](../ratetype/)
* class [RateByDateCollection](../ratebydatecollection/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


