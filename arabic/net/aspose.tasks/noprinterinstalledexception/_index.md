---
title: "الفئة NoPrinterInstalledException"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.NoPrinterInstalledException. تمثل استثناءً يُرمى عندما لا يوجد طابعة مثبتة في نظام التشغيل."
type: docs
weight: 1100
url: /ar/net/aspose.tasks/noprinterinstalledexception/
---
## NoPrinterInstalledException class

يمثل استثناءً يُرمى عندما لا يوجد طابعة مثبتة في نظام التشغيل.

```csharp
public class NoPrinterInstalledException : Exception
```

## الأمثلة

يوضح كيفية استخدام خيارات الطباعة.

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

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


