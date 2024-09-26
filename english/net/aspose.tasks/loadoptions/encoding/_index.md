---
title: LoadOptions.Encoding
second_title: Aspose.Tasks for .NET API Reference
description: LoadOptions property. Gets or sets encoding which is used to read a project from HTML MPX XER and Primavera XML formats. The default encoding is UTF8
type: docs
weight: 30
url: /net/aspose.tasks/loadoptions/encoding/
---
## LoadOptions.Encoding property

Gets or sets encoding which is used to read a project from HTML, MPX, XER and Primavera XML formats. The default encoding is UTF8.

```csharp
public Encoding Encoding { get; set; }
```

## Examples

Shows how to specify encoding when opening a project from Primavera XER file.

```csharp
LoadOptions lo = new LoadOptions();
lo.Encoding = Encoding.GetEncoding(1251);
lo.PrimaveraReadOptions = new PrimaveraReadOptions();
var project = new Project("encoding1251.xer", lo);
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


