---
title: "CopyToOptions.CopyToOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CopyToOptions 构造函数。初始化 CopyToOptions 类的新实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks/copytooptions/copytooptions/
---
## CopyToOptions constructor

初始化 [`CopyToOptions`](../) 类的新实例。

```csharp
public CopyToOptions()
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


