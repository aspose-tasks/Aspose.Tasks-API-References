---
title: PrintOptions.PrintOptions
second_title: Aspose.Tasks for .NET API Reference
description: PrintOptions constructor. Initializes a new instance of the PrintOptions class that can be used to set different options to print project
type: docs
weight: 10
url: /net/aspose.tasks.saving/printoptions/printoptions/
---
## PrintOptions constructor

Initializes a new instance of the [`PrintOptions`](../) class that can be used to set different options to print project.

```csharp
public PrintOptions()
```

## Examples

Shows how to use print options.

```csharp
try
{
    var project = new Project(DataDir + "Project2.mpp");
    var options = new PrintOptions
    {
        Timescale = Timescale.ThirdsOfMonths
    };
    if (project.GetPageCount(Timescale.ThirdsOfMonths) <= 280)
    {
        project.Print(options);
    }
}
catch (NoPrinterInstalledException ex)
{
    Console.WriteLine(ex.Message);
}
```

### See Also

* class [PrintOptions](../)
* namespace [Aspose.Tasks.Saving](../../printoptions/)
* assembly [Aspose.Tasks](../../../)


