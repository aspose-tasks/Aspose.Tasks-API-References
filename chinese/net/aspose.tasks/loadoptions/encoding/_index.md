---
title: "LoadOptions.Encoding"
second_title: "Aspose.Tasks for .NET API 参考"
description: "LoadOptions 属性。获取或设置用于从 HTML、MPX、XER 和 Primavera XML 格式读取项目的编码。默认编码为 UTF8。"
type: docs
weight: 30
url: /zh/net/aspose.tasks/loadoptions/encoding/
---
## LoadOptions.Encoding property

获取或设置用于从 HTML、MPX、XER 和 Primavera XML 格式读取项目的编码。默认编码为 UTF8。

```csharp
public Encoding Encoding { get; set; }
```

## 示例

展示如何在从 Primavera XER 文件打开项目时指定编码。

```csharp
LoadOptions lo = new LoadOptions();
lo.Encoding = Encoding.GetEncoding(1251);
lo.PrimaveraReadOptions = new PrimaveraReadOptions();
var project = new Project("encoding1251.xer", lo);
```

### 另见

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


