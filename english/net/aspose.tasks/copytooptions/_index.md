---
title: Class CopyToOptions
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.CopyToOptions class. Allows to specify additional options when copying project data
type: docs
weight: 340
url: /net/aspose.tasks/copytooptions/
---
## CopyToOptions class

Allows to specify additional options when copying project data.

```csharp
public class CopyToOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [CopyToOptions](copytooptions/)() | Initializes a new instance of the `CopyToOptions` class. |

## Properties

| Name | Description |
| --- | --- |
| [CopyViewData](../../aspose.tasks/copytooptions/copyviewdata/) { get; set; } | Gets or sets a value indicating whether to copy view data while copying project data. Default value is true. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


