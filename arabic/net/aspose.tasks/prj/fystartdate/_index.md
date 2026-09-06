---
title: "Prj.FyStartDate"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. الشهر الذي يبدأ فيه السنة المالية"
type: docs
weight: 350
url: /ar/net/aspose.tasks/prj/fystartdate/
---
## Prj.FyStartDate field

الشهر الذي يبدأ فيه السنة المالية.

```csharp
public static readonly Key<Month, PrjKey> FyStartDate;
```

## الأمثلة

يُظهر كيفية كتابة خصائص السنة المالية.

```csharp
var project = new Project(DataDir + "WriteFiscalYearProperties.mpp");

// تعيين خصائص السنة المالية
project.Set(Prj.FyStartDate, Month.July);
project.Set(Prj.FiscalYearStart, true);

// عرض خصائص السنة المالية
Console.WriteLine("Fiscal Year Start Date: " + project.Get(Prj.FyStartDate));
Console.WriteLine("Fiscal Year Numbering: " + project.Get(Prj.FiscalYearStart));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [Month](../../month/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


