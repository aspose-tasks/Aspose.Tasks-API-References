---
title: "枚举 ResourceType"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ResourceType 枚举。指定资源的类型"
type: docs
weight: 1800
url: /zh/net/aspose.tasks/resourcetype/
---
## ResourceType enumeration

指定资源的类型。

```csharp
public enum ResourceType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Material | `0` | 指示材料资源类型。 |
| Work | `1` | 指示工作资源类型。 |
| Cost | `2` | 指示成本资源类型。 |

## 示例

展示如何使用资源类型。

```csharp
var project = new Project();

// 添加工作资源
var work = project.Resources.Add("Work resource");
work.Set(Rsc.Type, ResourceType.Work);

// 添加材料资源
var material = project.Resources.Add("Material resource");
material.Set(Rsc.Type, ResourceType.Material);
material.Set(Rsc.MaterialLabel, "kg");

// 添加材料资源
var cost = project.Resources.Add("Cost resource");
cost.Set(Rsc.Type, ResourceType.Cost);
cost.Set(Rsc.Cost, 59.99m);

// 使用资源：创建任务、分配资源等...
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


