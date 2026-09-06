---
title: "PrimaveraXmlSaveOptions.SaveRootTask"
second_title: "Aspose.Tasks for .NET API 参考"
description: "PrimaveraXmlSaveOptions 属性。获取或设置指示是否保存根任务的值"
type: docs
weight: 20
url: /zh/net/aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/
---
## PrimaveraXmlSaveOptions.SaveRootTask property

获取或设置一个值，指示是否保存根任务。

```csharp
public bool SaveRootTask { get; set; }
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


