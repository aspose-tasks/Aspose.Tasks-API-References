---
title: "Rsc.HyperlinkSubAddress"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Rsc field. الموقع المحدد في مستند داخل ارتباط تشعبي مرتبط بالمهمة"
type: docs
weight: 340
url: /ar/net/aspose.tasks/rsc/hyperlinksubaddress/
---
## Rsc.HyperlinkSubAddress field

الموقع المحدد في المستند داخل الرابط المرتبط بمهمة.

```csharp
public static readonly Key<string, RscKey> HyperlinkSubAddress;
```

## ملاحظات

العنوان الكامل (Hyperlink Href في Microsoft Project) للرابط التشعبي هو دمج بين HyperlinkAddress و HyperlinkSubAddress.

## الأمثلة

يوضح كيفية قراءة/كتابة خصائص الروابط التشعبية للمورد.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Hyperlink, "Click to visit our site");
resource.Set(Rsc.HyperlinkAddress, "https://products.aspose.com");
resource.Set(Rsc.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + resource.Get(Rsc.Hyperlink));
Console.WriteLine("Hyperlink Address: " + resource.Get(Rsc.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + resource.Get(Rsc.HyperlinkSubAddress));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


