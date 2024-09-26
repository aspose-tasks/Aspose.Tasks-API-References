---
title: PrimaveraXmlSaveOptions.PrimaveraXmlSaveOptions
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraXmlSaveOptions constructor. Initializes a new instance of the PrimaveraXmlSaveOptions class
type: docs
weight: 10
url: /net/aspose.tasks.saving/primaveraxmlsaveoptions/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions constructor

Initializes a new instance of the [`PrimaveraXmlSaveOptions`](../) class.

```csharp
public PrimaveraXmlSaveOptions()
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


