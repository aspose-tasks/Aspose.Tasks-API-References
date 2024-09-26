---
title: CopyToOptions.CopyViewData
second_title: Aspose.Tasks for .NET API Reference
description: CopyToOptions property. Gets or sets a value indicating whether to copy view data while copying project data. Default value is true
type: docs
weight: 20
url: /net/aspose.tasks/copytooptions/copyviewdata/
---
## CopyToOptions.CopyViewData property

Gets or sets a value indicating whether to copy view data while copying project data. Default value is true.

```csharp
public bool CopyViewData { get; set; }
```

## Examples

Shows how to use project copy options.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// skip copying of view data while copying common project data.
var copyToOptions = new CopyToOptions();
copyToOptions.CopyViewData = false;
project.CopyTo(mppProject, copyToOptions);
```

### See Also

* class [CopyToOptions](../)
* namespace [Aspose.Tasks](../../copytooptions/)
* assembly [Aspose.Tasks](../../../)


