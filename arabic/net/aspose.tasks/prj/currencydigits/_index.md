---
title: "Prj.CurrencyDigits"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. عدد الأرقام بعد الفاصل العشري"
type: docs
weight: 160
url: /ar/net/aspose.tasks/prj/currencydigits/
---
## Prj.CurrencyDigits field

عدد الأرقام بعد الفاصل العشري.

```csharp
public static readonly Key<int, PrjKey> CurrencyDigits;
```

## الأمثلة

يظهر كيفية كتابة خصائص عملة المشروع.

```csharp
var project = new Project(DataDir + "WriteCurrencyProperties.mpp");

// تعيين خصائص العملة
project.Set(Prj.CurrencyCode, "AUD");
project.Set(Prj.CurrencyDigits, 2);
project.Set(Prj.CurrencySymbol, "$");
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.After);

// عرض خصائص العملة
Console.WriteLine("Currency Code: " + project.Get(Prj.CurrencyCode));
Console.WriteLine("Currency Digits: " + project.Get(Prj.CurrencyDigits));
Console.WriteLine("Currency Symbol: " + project.Get(Prj.CurrencySymbol));
Console.WriteLine("Currency Symbol Position: " + project.Get(Prj.CurrencySymbolPosition));

project.Save(OutDir + "WriteCurrencyProperties_out.xml", SaveFileFormat.Xml);
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


