---
title: "Filter.Equals"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Filter 方法。返回一个值，指示此实例是否等于指定的 AssignmentBaseline 对象。"
type: docs
weight: 100
url: /zh/net/aspose.tasks/filter/equals/
---
## Equals(Filter) {#equals}

返回一个值，指示此实例是否等于指定的 AssignmentBaseline 对象。

```csharp
public bool Equals(Filter other)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 其他 | Filter | 用于与此实例比较的指定 AssignmentBaseline 对象。 |

### 返回值

如果此实例等于指定的 AssignmentBaseline 对象则返回 true；否则返回 false。

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

---

## Equals(object) {#equals_1}

返回一个值，指示此实例是否等于指定的 AssignmentBaseline 对象。

```csharp
public override bool Equals(object obj)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | 对象 | 用于与此实例比较的指定 AssignmentBaseline 对象。 |

### 返回值

如果此实例等于指定的 AssignmentBaseline 对象则返回 true；否则返回 false。

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


