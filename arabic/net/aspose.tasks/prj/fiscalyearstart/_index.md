---
title: "Prj.FiscalYearStart"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كان يتم استخدام ترقيم السنة المالية"
type: docs
weight: 340
url: /ar/net/aspose.tasks/prj/fiscalyearstart/
---
## Prj.FiscalYearStart field

يحدد ما إذا كان يتم استخدام ترقيم السنة المالية.

```csharp
public static readonly Key<NullableBool, PrjKey> FiscalYearStart;
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
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


