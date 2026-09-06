---
title: "Duration.GetHashCode"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Duration 方法。返回此对象的哈希码值。"
type: docs
weight: 90
url: /zh/net/aspose.tasks/duration/gethashcode/
---
## Duration.GetHashCode method

返回此对象的哈希码值。

```csharp
public override int GetHashCode()
```

### 返回值

返回此 Duration 实例的哈希码值。

## 示例

展示如何获取 Duration 的哈希码。

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// 日历的哈希码基于时间单位类型和 Duration 的初始值。
// 因此后续的哈希码相等。
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 2 Hash Code: {0}", duration2.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration2.GetHashCode()));

// 但 Duration 1 和 3 的哈希码不相等。
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 3 Hash Code: {0}", duration3.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration3.GetHashCode()));
```

### 另见

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


