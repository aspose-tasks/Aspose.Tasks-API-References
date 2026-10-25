---
title: "枚举 EarnedValueMethodType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.EarnedValueMethodType 枚举。指定用于计算挣值的方法"
type: docs
weight: 480
url: /zh/net/aspose.tasks/earnedvaluemethodtype/
---
## EarnedValueMethodType enumeration

指定用于计算挣值的方法。

```csharp
public enum EarnedValueMethodType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Undefined | `-1` | 该字段未在原始项目文件中定义。 |
| PercentComplete | `0` | 完成百分比 |
| PhysicalPercentComplete | `1` | 实际完成百分比 |

## 备注

在导出为 XML 时，未定义的值将从生成的 XML 中删除。

## 示例

展示如何指定用于计算挣值的方法 (EarnedValueMethodType.PercentComplete)。

```csharp
var project = new Project(DataDir + "Project2.mpp");
// 将挣值方法类型设置为 'PercentComplete'
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
// 处理项目...
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


