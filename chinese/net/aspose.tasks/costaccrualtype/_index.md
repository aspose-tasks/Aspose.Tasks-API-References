---
title: "枚举 CostAccrualType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.CostAccrualType 枚举。指定累计成本的类型"
type: docs
weight: 350
url: /zh/net/aspose.tasks/costaccrualtype/
---
## CostAccrualType enumeration

指定累计成本的类型。

```csharp
public enum CostAccrualType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Undefined | `-1` | 指示未定义值表示该字段在原始项目文件中未定义。 |
| Start | `0` | 指示开始成本累计类型。 |
| Prorated | `1` | 指示按比例分配的成本累计类型。 |
| End | `2` | 指示结束成本累计类型。 |
| Invalid | `3` | 指示无效的成本累计类型。 |

## 备注

在导出为 XML 时，未定义的值将从生成的 XML 中删除。

## 示例

展示资源标准成本和加班成本何时以及如何被计费或累计（累计方式：确定资源成本何时产生以及实际成本何时计入项目。您可以在任务的开始 [Start] 或结束 [End] 时产生成本，或在任务期间按比例 [Prorated] 产生成本），用于任务的成本 (CostAccrualType.End)。

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);
// 设置成本累计类型
// 如果选择结束选项，成本将在剩余工作为零之前不被累计。
resource.Set(Rsc.AccrueAt, CostAccrualType.End);
// 处理项目...
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


