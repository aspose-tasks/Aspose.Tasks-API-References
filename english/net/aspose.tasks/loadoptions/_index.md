---
title: Class LoadOptions
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.LoadOptions class. Allows to specify additional load parameters when loading a project from file or stream
type: docs
weight: 980
url: /net/aspose.tasks/loadoptions/
---
## LoadOptions class

Allows to specify additional load parameters when loading a project from file or stream.

```csharp
public class LoadOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [LoadOptions](loadoptions/)() | Initializes a new instance of the `LoadOptions` class. |

## Properties

| Name | Description |
| --- | --- |
| [CancellationToken](../../aspose.tasks/loadoptions/cancellationtoken/) { get; set; } | Gets or sets a token which can be used to cancel a project loading operation. |
| [Encoding](../../aspose.tasks/loadoptions/encoding/) { get; set; } | Gets or sets encoding which is used to read a project from HTML, MPX, XER and Primavera XML formats. The default encoding is UTF8. |
| [ErrorHandler](../../aspose.tasks/loadoptions/errorhandler/) { get; set; } | Gets or sets a callback method to handle xml parse errors. |
| [Password](../../aspose.tasks/loadoptions/password/) { get; set; } | Gets or sets a protection password. |
| [PrimaveraReadOptions](../../aspose.tasks/loadoptions/primaverareadoptions/) { get; set; } | Gets or sets a specified instance of the [`PrimaveraReadOptions`](../primaverareadoptions/) class which can be used to customize the behavior of loading Primavera formats (Primavera P6 XER or Primavera P6 Xml). |

## Examples

Shows how to load the password-protected project using &lt;see cref="Aspose.Tasks.LoadOptions"/&gt; instance.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


