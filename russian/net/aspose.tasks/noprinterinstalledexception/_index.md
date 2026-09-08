---
title: "Класс NoPrinterInstalledException"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.NoPrinterInstalledException. Представляет исключение, которое выбрасывается, когда в ОС нет установленного принтера."
type: docs
weight: 1100
url: /ru/net/aspose.tasks/noprinterinstalledexception/
---
## NoPrinterInstalledException class

Представляет исключение, которое бросается, когда в ОС нет установленного принтера.

```csharp
public class NoPrinterInstalledException : Exception
```

## Примеры

Показывает, как использовать параметры печати.

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

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


