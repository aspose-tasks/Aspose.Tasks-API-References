---
title: PrimaveraXmlSaveOptions.SaveRootTask
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraXmlSaveOptions property. Gets or sets a value indicating whether to save a root task or not
type: docs
weight: 20
url: /net/aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/
---
## PrimaveraXmlSaveOptions.SaveRootTask property

Gets or sets a value indicating whether to save a root task or not.

```csharp
public bool SaveRootTask { get; set; }
```

## Examples

Shows how to export the to Primavera XML file.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### See Also

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


