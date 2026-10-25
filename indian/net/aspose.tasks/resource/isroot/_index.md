---
title: "Resource.IsRoot"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Resource प्रॉपर्टी। यह फ़्लैग प्राप्त करता है जो दर्शाता है कि संसाधन रूट संसाधन है या नहीं। रूट संसाधन एक विशेष संसाधन है जो MS Projects फ़ॉर्मेट के आंतरिक हिस्सों को समर्थन देने के लिए बनाया गया है और उपयोगकर्ता कोड से सीधे उपयोग करने के लिए नहीं है।"
type: docs
weight: 470
url: /hi/net/aspose.tasks/resource/isroot/
---
## Resource.IsRoot property

प्राप्त करता है वह फ़्लैग जो यह दर्शाता है कि संसाधन एक मूल (रूट) संसाधन है या नहीं। मूल संसाधन एक विशेष संसाधन है जिसे MS Project के फ़ॉर्मेट्स के आंतरिक भागों को समर्थन देने के लिए बनाया गया है और इसे उपयोगकर्ता के कोड से सीधे उपयोग करने के लिए नहीं बनाया गया है।

```csharp
public virtual bool IsRoot { get; }
```

## उदाहरण

रूट संसाधन को छोड़ने के लिए IsRoot प्रॉपर्टी का उपयोग कैसे करें, यह दिखाता है।

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

foreach (var resource in project.Resources)
{
    if (resource.IsRoot)
    {
        continue;
    }

    Console.WriteLine(resource.Get(Rsc.Name));
}
```

### संबंधित देखें

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


