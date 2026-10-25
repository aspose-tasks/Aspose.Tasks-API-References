---
title: "Rsc.HyperlinkAddress"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. العنوان لرابط تشعبي مرتبط بمورد"
type: docs
weight: 330
url: /ar/net/aspose.tasks/rsc/hyperlinkaddress/
---
## Rsc.HyperlinkAddress field

العنوان الخاص بالرابط المرتبط بالمورد.

```csharp
public static readonly Key<string, RscKey> HyperlinkAddress;
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


