---
title: CopyToOptions.CopyToOptions
second_title: Aspose.Tasks for .NET API Reference
description: CopyToOptions constructor. Initializes a new instance of the CopyToOptions class
type: docs
weight: 10
url: /net/aspose.tasks/copytooptions/copytooptions/
---
## CopyToOptions constructor

Initializes a new instance of the [`CopyToOptions`](../) class.

```csharp
public CopyToOptions()
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


