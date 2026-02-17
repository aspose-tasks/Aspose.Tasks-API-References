---
title: Class NoPrinterInstalledException
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.NoPrinterInstalledException class. Represents an exception which is thrown when there is no installed printer in OS
type: docs
weight: 1090
url: /net/aspose.tasks/noprinterinstalledexception/
---
## NoPrinterInstalledException class

Represents an exception which is thrown when there is no installed printer in OS.

```csharp
public class NoPrinterInstalledException : Exception
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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


