---
title: "CopyToOptions.CopyViewData"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CopyToOptions 属性。获取或设置一个值，指示在复制项目数据时是否复制视图数据。默认值为 true"
type: docs
weight: 20
url: /zh/net/aspose.tasks/copytooptions/copyviewdata/
---
## CopyToOptions.CopyViewData property

获取或设置一个值，指示在复制项目数据时是否复制视图数据。默认值为 true。

```csharp
public bool CopyViewData { get; set; }
```

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

* class [CopyToOptions](../)
* namespace [Aspose.Tasks](../../copytooptions/)
* assembly [Aspose.Tasks](../../../)


