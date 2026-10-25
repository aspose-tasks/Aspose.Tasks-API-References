---
title: "LoadOptions.CancellationToken"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية LoadOptions. تحصل أو تعيّن رمزًا يمكن استخدامه لإلغاء عملية تحميل المشروع."
type: docs
weight: 20
url: /ar/net/aspose.tasks/loadoptions/cancellationtoken/
---
## LoadOptions.CancellationToken property

يحصل أو يعيّن رمزًا يمكن استخدامه لإلغاء عملية تحميل المشروع.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## الأمثلة

يوضح كيفية تمرير CancellationToken لإلغاء عملية تحميل مشروع طويلة الأمد.

```csharp
var loadOptions = new LoadOptions();

CancellationTokenSource cts = new CancellationTokenSource();
loadOptions.CancellationToken = cts.Token;

// يمكن تمرير cts إلى خيط آخر حيث يمكن استدعاء الطريقة cts.Cancel() لإلغاء عملية تحميل المشروع.
// cts.Cancel();
var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
```

### انظر أيضًا

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


