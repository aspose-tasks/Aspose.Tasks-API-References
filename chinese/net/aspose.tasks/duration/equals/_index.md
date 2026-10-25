---
title: "Duration.Equals"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Duration 方法。返回一个值，指示此实例是否等于指定的对象。"
type: docs
weight: 80
url: /zh/net/aspose.tasks/duration/equals/
---
## Equals(Duration) {#equals}

返回一个值，指示此实例是否等于指定的对象。

```csharp
public bool Equals(Duration other)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 其他 | 持续时间 | 与此实例比较的对象。 |

### 返回值

如果其他 Duration 实例具有与此实例相同的 TimeSpan 和 TimeUnit 值，则返回 **True**；否则返回 **false**。

## 示例

展示如何检查 Duration 相等性。

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// Duration 的相等性是相对于底层 TimeSpan 进行检查的。
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### 另见

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

返回一个值，指示此实例是否等于指定的对象。

```csharp
public override bool Equals(object obj)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | 对象 | 与此实例比较的对象。 |

### 返回值

**True** if the specified object is a Duration that has the same TimeSpan and TimeUnit values as this instance; otherwise, **false**.

## 示例

展示如何检查 Duration 相等性。

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// Duration 的相等性是相对于底层 TimeSpan 进行检查的。
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### 另见

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


