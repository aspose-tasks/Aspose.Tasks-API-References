---
title: "Tsk.Hyperlink"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Tsk. العنوان أو النص التوضيحي لرابط تشعبي مرتبط بمهمة."
type: docs
weight: 490
url: /ar/net/aspose.tasks/tsk/hyperlink/
---
## Tsk.Hyperlink field

العنوان أو النص التوضيحي للرابط المرتبط بمهمة.

```csharp
public static readonly Key<string, TaskKey> Hyperlink;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خصائص Tsk.Hyperlink.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Hyperlink, "Click here to visit our site");
task.Set(Tsk.HyperlinkAddress, "https://products.aspose.com");
task.Set(Tsk.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + task.Get(Tsk.Hyperlink));
Console.WriteLine("Hyperlink Address: " + task.Get(Tsk.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + task.Get(Tsk.HyperlinkSubAddress));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


