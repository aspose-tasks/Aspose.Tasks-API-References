---
title: "Rsc.IsNull"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। निर्धारित करता है कि कोई संसाधन null है या नहीं"
type: docs
weight: 420
url: /hi/net/aspose.tasks/rsc/isnull/
---
## Rsc.IsNull field

निर्धारित करता है कि संसाधन शून्य है या नहीं।

```csharp
public static readonly Key<NullableBool, RscKey> IsNull;
```

## उदाहरण

दिखाता है कि Rsc.IsNull प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsNull, true);

Console.WriteLine("Is Null: " + resource.Get(Rsc.IsNull));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


