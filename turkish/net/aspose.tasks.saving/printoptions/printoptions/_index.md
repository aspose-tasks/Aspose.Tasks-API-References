---
title: "PrintOptions.PrintOptions"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "PrintOptions yapıcı. Projeyi yazdırmak için farklı seçenekler ayarlamak amacıyla kullanılabilecek PrintOptions sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks.saving/printoptions/printoptions/
---
## PrintOptions constructor

[`PrintOptions`](../) sınıfının yeni bir örneğini başlatır; bu, projeyi yazdırmak için farklı seçenekler ayarlamakta kullanılabilir.

```csharp
public PrintOptions()
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

* class [PrintOptions](../)
* namespace [Aspose.Tasks.Saving](../../printoptions/)
* assembly [Aspose.Tasks](../../../)


