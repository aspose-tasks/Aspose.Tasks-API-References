---
title: "Duration.ParseTimeSpan"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Duration 方法。解析格式为 PTHMS 的持续时间字符串。"
type: docs
weight: 130
url: /zh/net/aspose.tasks/duration/parsetimespan/
---
## Duration.ParseTimeSpan method

解析格式为 "PT--H--M--S--" 的持续时间字符串。

```csharp
public static TimeSpan ParseTimeSpan(string value)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | 字符串 | 要解析的指定字符串。 |

### 返回值

返回已解析的 [`TimeSpan`](../timespan/) 结构体实例。

## 示例

展示如何将字符串转换为时间跨度。

```csharp
var timeSpan = Duration.ParseTimeSpan("PT1H10M30S");
Console.WriteLine("The parsed time span: " + timeSpan);
```

### 另见

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


