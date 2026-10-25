---
title: "PrimaveraXmlSaveOptions.PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PrimaveraXmlSaveOptions 构造函数。初始化一个新的 PrimaveraXmlSaveOptions 类实例"
type: docs
weight: 10
url: /zh/net/aspose.tasks.saving/primaveraxmlsaveoptions/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions constructor

初始化一个新的 [`PrimaveraXmlSaveOptions`](../) 类实例。

```csharp
public PrimaveraXmlSaveOptions()
```

## 示例

展示如何导出到 Primavera XML 文件。

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### 另见

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


