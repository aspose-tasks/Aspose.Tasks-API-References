---
title: "枚举 BaselineType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.BaselineType 枚举。指定用于计算差异值的基线类型"
type: docs
weight: 130
url: /zh/net/aspose.tasks/baselinetype/
---
## BaselineType enumeration

指定用于计算差异值的基线类型。

```csharp
public enum BaselineType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Undefined | `-1` | 指示该字段在原始项目文件中未定义。 |
| Baseline | `0` | 指示基线类型。 |
| Baseline1 | `1` | 指示 Baseline1 类型。 |
| Baseline2 | `2` | 指示 Baseline2 类型。 |
| Baseline3 | `3` | 指示 Baseline3 类型。 |
| Baseline4 | `4` | 指示 Baseline4 类型。 |
| Baseline5 | `5` | 指示 Baseline5 类型。 |
| Baseline6 | `6` | 指示 Baseline6 类型。 |
| Baseline7 | `7` | 指示 Baseline7 类型。 |
| Baseline8 | `8` | 指示 Baseline8 类型。 |
| Baseline9 | `9` | 指示 Baseline9 类型。 |
| Baseline10 | `10` | 指示 Baseline10 类型。 |

## 备注

在导出为 XML 时，未定义的值将从生成的 XML 中删除。

## 示例

展示如何为项目设置基线 (BaselineType.Baseline)。

```csharp
var project = new Project(DataDir + "Project2.mpp");
// 将基线字段保存到整个项目的指定基线。
project.SetBaseline(BaselineType.Baseline);
// 处理项目的基线……
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


