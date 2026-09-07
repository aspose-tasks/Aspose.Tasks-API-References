---
title: "Prj.Autolink"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। निर्धारित करता है कि सम्मिलित या स्थानांतरित कार्य स्वतः लिंक किए जाते हैं या नहीं"
type: docs
weight: 70
url: /hi/net/aspose.tasks/prj/autolink/
---
## Prj.Autolink field

निर्धारित करता है कि सम्मिलित या स्थानांतरित कार्य स्वचालित रूप से जुड़े हैं या नहीं।

```csharp
public static readonly Key<NullableBool, PrjKey> Autolink;
```

## उदाहरण

दिखाता है कि Prj.Autolink प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.Autolink, true);

Console.WriteLine("Autolink: " + project.Get(Prj.Autolink));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


