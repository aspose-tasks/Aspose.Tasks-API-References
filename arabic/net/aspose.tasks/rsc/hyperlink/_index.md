---
title: "Rsc.Hyperlink"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. العنوان أو النص التوضيحي لرابط تشعبي مرتبط بمورد"
type: docs
weight: 320
url: /ar/net/aspose.tasks/rsc/hyperlink/
---
## Rsc.Hyperlink field

العنوان أو النص التوضيحي للرابط المرتبط بالمورد.

```csharp
public static readonly Key<string, RscKey> Hyperlink;
```

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


