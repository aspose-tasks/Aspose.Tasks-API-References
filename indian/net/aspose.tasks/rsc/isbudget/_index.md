---
title: "Rsc.IsBudget"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc field. निर्धारित करता है कि क्या कार्य सामग्री या लागत संसाधन बजट संसाधन है"
type: docs
weight: 380
url: /hi/net/aspose.tasks/rsc/isbudget/
---
## Rsc.IsBudget field

निर्धारित करता है कि कार्य, सामग्री या लागत संसाधन बजट संसाधन है या नहीं।

```csharp
public static readonly Key<NullableBool, RscKey> IsBudget;
```

## उदाहरण

दिखाता है कि Rsc.IsBudget प्रॉपर्टी को कैसे पढ़ें/लिखें.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsBudget, true);

Console.WriteLine("Is Budget: " + resource.Get(Rsc.IsBudget));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


