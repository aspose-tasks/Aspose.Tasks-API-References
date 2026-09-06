---
title: "Rsc.StandardRateFormat"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. الوحدات المستخدمة في Microsoft Project لعرض السعر القياسي"
type: docs
weight: 630
url: /ar/net/aspose.tasks/rsc/standardrateformat/
---
## Rsc.StandardRateFormat field

الوحدات التي يستخدمها Microsoft Project لعرض المعدل القياسي.

```csharp
public static readonly Key<RateFormatType, RscKey> StandardRateFormat;
```

## الأمثلة

يوضح كيفية قراءة/كتابة الخاصية Rsc.StandardRateFormat.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


