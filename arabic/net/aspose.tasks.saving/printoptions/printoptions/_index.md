---
title: "PrintOptions.PrintOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ PrintOptions. يهيئ مثيلاً جديداً لفئة PrintOptions يمكن استخدامها لتعيين خيارات مختلفة لطباعة المشروع"
type: docs
weight: 10
url: /ar/net/aspose.tasks.saving/printoptions/printoptions/
---
## PrintOptions constructor

يهيئ مثيلاً جديداً لفئة [`PrintOptions`](../) يمكن استخدامها لتعيين خيارات مختلفة لطباعة المشروع.

```csharp
public PrintOptions()
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

* class [PrintOptions](../)
* namespace [Aspose.Tasks.Saving](../../printoptions/)
* assembly [Aspose.Tasks](../../../)


