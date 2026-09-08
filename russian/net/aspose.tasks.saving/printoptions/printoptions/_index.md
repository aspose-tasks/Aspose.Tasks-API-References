---
title: "PrintOptions.PrintOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор PrintOptions. Инициализирует новый экземпляр класса PrintOptions, который может использоваться для установки различных параметров печати проекта."
type: docs
weight: 10
url: /ru/net/aspose.tasks.saving/printoptions/printoptions/
---
## PrintOptions constructor

Инициализирует новый экземпляр класса [`PrintOptions`](../), который может использоваться для установки различных параметров печати проекта.

```csharp
public PrintOptions()
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

* class [PrintOptions](../)
* namespace [Aspose.Tasks.Saving](../../printoptions/)
* assembly [Aspose.Tasks](../../../)


