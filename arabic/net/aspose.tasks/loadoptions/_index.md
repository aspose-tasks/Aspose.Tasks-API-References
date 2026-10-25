---
title: "الفئة LoadOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.LoadOptions. تسمح بتحديد معلمات تحميل إضافية عند تحميل مشروع من ملف أو تدفق."
type: docs
weight: 990
url: /ar/net/aspose.tasks/loadoptions/
---
## LoadOptions class

يسمح بتحديد معلمات تحميل إضافية عند تحميل مشروع من ملف أو تدفق.

```csharp
public class LoadOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [LoadOptions](loadoptions/)() | ينشئ مثيلًا جديدًا من الفئة `LoadOptions`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CancellationToken](../../aspose.tasks/loadoptions/cancellationtoken/) { get; set; } | يحصل أو يعيّن رمزًا يمكن استخدامه لإلغاء عملية تحميل المشروع. |
| [Encoding](../../aspose.tasks/loadoptions/encoding/) { get; set; } | يحصل أو يعيّن الترميز المستخدم لقراءة مشروع من صيغ HTML، MPX، XER وPrimavera XML. الترميز الافتراضي هو UTF8. |
| [ErrorHandler](../../aspose.tasks/loadoptions/errorhandler/) { get; set; } | يحصل أو يعيّن طريقة رد نداء للتعامل مع أخطاء تحليل XML. |
| [Password](../../aspose.tasks/loadoptions/password/) { get; set; } | يحصل أو يعيّن كلمة مرور الحماية. |
| [PrimaveraReadOptions](../../aspose.tasks/loadoptions/primaverareadoptions/) { get; set; } | يحصل أو يعيّن مثيلًا محددًا من الفئة [`PrimaveraReadOptions`](../primaverareadoptions/) الذي يمكن استخدامه لتخصيص سلوك تحميل صيغ Primavera (Primavera P6 XER أو Primavera P6 Xml). |
| [ProjectLoadingCallback](../../aspose.tasks/loadoptions/projectloadingcallback/) { get; set; } | يحصل أو يعيّن رد النداء الذي يتم استدعاؤه أثناء عمليات تحميل المشروع. مدعوم حاليًا لصيغ MPP و XER. |

## الأمثلة

يوضح كيفية تحميل المشروع المحمي بكلمة مرور باستخدام &lt;see cref=\"Aspose.Tasks.LoadOptions\"/&gt;.

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


