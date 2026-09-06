---
title: "枚举 CurrencySymbolPositionType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.CurrencySymbolPositionType 枚举。指定货币符号的位置。"
type: docs
weight: 370
url: /zh/net/aspose.tasks/currencysymbolpositiontype/
---
## CurrencySymbolPositionType enumeration

指定货币符号的位置。

```csharp
public enum CurrencySymbolPositionType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Undefined | `-1` | 指示未定义值表示该字段在原始项目文件中未定义。 |
| Before | `0` | 指示货币符号前置的位置类型。 |
| After | `1` | 指示货币符号后置的位置类型。 |
| BeforeWithSpace | `2` | 指示货币符号前置并带空格的位置类型。 |
| AfterWithSpace | `3` | 指示货币符号后置并带空格的位置类型。 |

## 备注

在导出为 XML 时，未定义的值将从生成的 XML 中删除。

## 示例

展示如何指定货币符号的放置位置（CurrencySymbolPositionType.Before）。

```csharp
var project = new Project(DataDir + "Project2.mpp");
// 设置货币符号的放置位置
// 前置，无空格 ($0)。
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.Before);
// 处理项目...
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


