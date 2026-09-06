---
title: "Duration.IsElapsed"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Duration 属性。获取指示时间单位是否已过去的值。决定此 Duration 实例是否已过去的标志。"
type: docs
weight: 20
url: /zh/net/aspose.tasks/duration/iselapsed/
---
## Duration.IsElapsed property

获取一个值，指示时间单位是否已过去。此标志决定此 Duration 实例是否已过去。

```csharp
public bool IsElapsed { get; }
```

## 示例

展示如何从特定格式的字符串解析字符串。

```csharp
var project = new Project();

// 持续时间示例：
// "1d", "1dy", "1d?", "1day", "1 dy", "1 edy? ", "8hr", "8 hour", "8hours", "0.2w?", "0.2wk", "0.2 eweek", "0.2ew?"
// 其中 1 - 项目数量（天、周等），d - 天（h - 小时，w - 周）? - 估计标志，e - 已过去标志

// 尝试解析估计的 Duration。
var duration1 = Duration.Parse(project, "1d?");
Console.WriteLine("The parsed time span: " + duration1.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration1.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration1.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration1.IsElapsed);
Console.WriteLine();

// 尝试解析估计的 Duration。
var duration2 = Duration.Parse(project, "0.2 eweek");
Console.WriteLine("The parsed time span: " + duration2.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration2.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration2.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration2.IsElapsed);
```

### 另见

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


