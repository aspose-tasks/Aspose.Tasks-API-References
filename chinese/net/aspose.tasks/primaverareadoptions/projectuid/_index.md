---
title: "PrimaveraReadOptions.ProjectUid"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PrimaveraReadOptions 属性。获取或设置要从包含多个项目的文件中读取的项目 UID。"
type: docs
weight: 30
url: /zh/net/aspose.tasks/primaverareadoptions/projectuid/
---
## PrimaveraReadOptions.ProjectUid property

获取或设置要从包含多个项目的文件中读取的项目 UID。

```csharp
public int ProjectUid { get; set; }
```

## 示例

展示如何从包含多个项目的 Primavera XML 或 Primavera XER 文件中读取项目。

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// 返回具有特殊 UID 的项目
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### 另见

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


