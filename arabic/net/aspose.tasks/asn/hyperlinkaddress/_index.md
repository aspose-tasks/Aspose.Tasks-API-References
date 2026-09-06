---
title: "Asn.HyperlinkAddress"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Asn field. العنوان لرابط تشعبي مرتبط بتعيين"
type: docs
weight: 290
url: /ar/net/aspose.tasks/asn/hyperlinkaddress/
---
## Asn.HyperlinkAddress field

العنوان للرابط المرتبط بالمهمة.

```csharp
public static readonly Key<string, AsnKey> HyperlinkAddress;
```

## ملاحظات

العنوان الكامل (Hyperlink Href في Microsoft Project) للرابط التشعبي هو دمج بين HyperlinkAddress و HyperlinkSubAddress.

## الأمثلة

يوضح كيفية قراءة/كتابة خصائص الرابط التشعبي.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Hyperlink, "Click to visit our site");
assignment.Set(Asn.HyperlinkAddress, "https://products.aspose.com");
assignment.Set(Asn.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + assignment.Get(Asn.Hyperlink));
Console.WriteLine("Hyperlink Address: " + assignment.Get(Asn.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + assignment.Get(Asn.HyperlinkSubAddress));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


