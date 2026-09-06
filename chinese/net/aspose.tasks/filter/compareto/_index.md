---
title: "Filter.CompareTo"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Filter 方法。比较此实例与指定的 Filter 类实例，并返回它们相对顺序的指示。"
type: docs
weight: 90
url: /zh/net/aspose.tasks/filter/compareto/
---
## Filter.CompareTo method

比较此实例与指定的 [`Filter`](../) 类实例，并返回它们相对顺序的指示。

```csharp
public int CompareTo(Filter other)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| other | Filter | 指定的 [`Filter`](../) 类实例以与此对象比较。 |

### 返回值

它们相对顺序的指示。

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


