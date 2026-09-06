---
title: "Project.SetBaselineSaveTime"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 方法。设置基线保存时间"
type: docs
weight: 1260
url: /zh/net/aspose.tasks/project/setbaselinesavetime/
---
## Project.SetBaselineSaveTime method

设置基线保存时间。

```csharp
public void SetBaselineSaveTime(BaselineType baselineNumber, DateTime value)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| baselineNumber | BaselineType | 基线的编号 [`BaselineType`](../../baselinetype/)。 |
| value | DateTime | 基线的最后保存日期和时间。 |

## 备注

如果基线未保存，则将值设为 DateTime.MinValue。

## 示例

展示如何读取/写入项目的基线保存时间。

```csharp
var project = new Project();
var baselineSave = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time before: " + baselineSave);

// 设置基线保存时间
project.SetBaselineSaveTime(BaselineType.Baseline, DateTime.Today);

var baselineSaveNew = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time after: " + baselineSaveNew);
```

### 另见

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


