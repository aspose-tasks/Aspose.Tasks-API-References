---
title: "Resource.IsRoot"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Resource. يحصل على العلامة التي تشير ما إذا كان المورد موردًا جذريًا. المورد الجذري هو مورد خاص يُقصد به دعم البُنى الداخلية لتنسيقات MS Projects ولا يُقصد استخدامه مباشرةً من كود المستخدم."
type: docs
weight: 470
url: /ar/net/aspose.tasks/resource/isroot/
---
## Resource.IsRoot property

يحصل على العلم الذي يشير إلى ما إذا كان المورد موردًا جذريًا. المورد الجذري هو مورد خاص يُقصد به دعم تفاصيل صيغ MS Project ولا يُقصد استخدامه مباشرةً من كود المستخدم.

```csharp
public virtual bool IsRoot { get; }
```

## الأمثلة

يوضح كيفية استخدام خاصية IsRoot لتخطي المورد الجذري.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

foreach (var resource in project.Resources)
{
    if (resource.IsRoot)
    {
        continue;
    }

    Console.WriteLine(resource.Get(Rsc.Name));
}
```

### انظر أيضًا

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


