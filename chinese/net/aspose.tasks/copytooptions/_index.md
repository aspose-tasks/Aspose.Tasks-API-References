---
title: "类 CopyToOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.CopyToOptions 类。允许在复制项目数据时指定附加选项"
type: docs
weight: 340
url: /zh/net/aspose.tasks/copytooptions/
---
## CopyToOptions class

允许在复制项目数据时指定附加选项。

```csharp
public class CopyToOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [CopyToOptions](copytooptions/)() | 初始化 `CopyToOptions` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [CopyViewData](../../aspose.tasks/copytooptions/copyviewdata/) { get; set; } | 获取或设置一个值，指示在复制项目数据时是否复制视图数据。默认值为 true。 |

## 示例

展示如何使用项目复制选项。

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// 在复制通用项目数据时跳过视图数据的复制。
var copyToOptions = new CopyToOptions();
copyToOptions.CopyViewData = false;
project.CopyTo(mppProject, copyToOptions);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


