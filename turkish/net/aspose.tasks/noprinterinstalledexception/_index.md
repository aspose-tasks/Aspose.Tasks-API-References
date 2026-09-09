---
title: "Sınıf NoPrinterInstalledException"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.NoPrinterInstalledException sınıfı. İşletim sisteminde yüklü bir yazıcı olmadığında fırlatılan bir istisnayı temsil eder"
type: docs
weight: 1100
url: /tr/net/aspose.tasks/noprinterinstalledexception/
---
## NoPrinterInstalledException class

İşletim sisteminde yüklü bir yazıcı olmadığında atılan bir istisnayı temsil eder.

```csharp
public class NoPrinterInstalledException : Exception
```

## Örnekler

Yazdırma seçeneklerini nasıl kullanacağınızı gösterir.

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

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


