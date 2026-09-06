---
title: "Filter.op_Equality"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Filter 方法。返回一个值，指示此实例是否等于指定的对象。"
type: docs
weight: 120
url: /zh/net/aspose.tasks/filter/op_equality/
---
## Filter Equality operator

返回一个值，指示此实例是否等于指定的对象。

```csharp
public static bool operator ==(Filter a, Filter b)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| a | Filter | 第一个过滤器。 |
| b | Filter | 第二个过滤器。 |

### 返回值

一个指示此实例是否等于指定对象的值。

## 示例

展示如何检查过滤器相等性。

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();

var filter1 = filters[0];
var filter2 = filters[1];

// 过滤器的相等性是根据过滤器的 UID 检查的。
Console.WriteLine("Filter 1 UID: " + filter1.Uid);
Console.WriteLine("Filter 2 UID: " + filter2.Uid);
Console.WriteLine("Are filters equal: " + filter1.Equals(filter2));
```

### 另见

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


