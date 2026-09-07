---
title: "Tsk.HyperlinkSubAddress"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य से जुड़ी हाइपरलिंक में दस्तावेज़ के भीतर विशिष्ट स्थान"
type: docs
weight: 510
url: /hi/net/aspose.tasks/tsk/hyperlinksubaddress/
---
## Tsk.HyperlinkSubAddress field

कार्य से जुड़े हाइपरलिंक में दस्तावेज़ का विशिष्ट स्थान।

```csharp
public static readonly Key<string, TaskKey> HyperlinkSubAddress;
```

## टिप्पणियाँ

हाइपरलिंक का पूर्ण पता (Microsoft Project में Hyperlink Href) HyperlinkAddress और HyperlinkSubAddress का संयोजन है।

## उदाहरण

दिखाता है कि Tsk.Hyperlink प्रॉपर्टीज़ को कैसे पढ़ें/लिखें।

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

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


