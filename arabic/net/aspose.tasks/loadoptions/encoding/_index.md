---
title: "LoadOptions.Encoding"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية LoadOptions. تحصل أو تعيّن الترميز الذي يُستخدم لقراءة مشروع من صيغ HTML MPX XER وPrimavera XML. الترميز الافتراضي هو UTF8"
type: docs
weight: 30
url: /ar/net/aspose.tasks/loadoptions/encoding/
---
## LoadOptions.Encoding property

يحصل أو يعيّن الترميز المستخدم لقراءة مشروع من صيغ HTML، MPX، XER وPrimavera XML. الترميز الافتراضي هو UTF8.

```csharp
public Encoding Encoding { get; set; }
```

## الأمثلة

يوضح كيفية تحديد الترميز عند فتح مشروع من ملف Primavera XER.

```csharp
LoadOptions lo = new LoadOptions();
lo.Encoding = Encoding.GetEncoding(1251);
lo.PrimaveraReadOptions = new PrimaveraReadOptions();
var project = new Project("encoding1251.xer", lo);
```

### انظر أيضًا

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


