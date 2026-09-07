---
title: "Prj.HonorConstraints"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। निर्धारित करता है कि कार्य अपने प्रतिबंध तिथियों का सम्मान करते हैं या नहीं।"
type: docs
weight: 370
url: /hi/net/aspose.tasks/prj/honorconstraints/
---
## Prj.HonorConstraints field

निर्धारित करता है कि कार्य अपनी बाधा तिथियों का सम्मान करते हैं या नहीं।

```csharp
public static readonly Key<NullableBool, PrjKey> HonorConstraints;
```

## उदाहरण

दिखाता है कि Prj.HonorConstraints प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

project.Set(Prj.HonorConstraints, true);

Console.WriteLine("Honor Constraints: " + project.Get(Prj.HonorConstraints));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


