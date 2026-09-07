---
title: "Metered.ResetMeteredKey"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Metered मेथड। पहले सेट की गई लाइसेंस को हटाता है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks/metered/resetmeteredkey/
---
## Metered.ResetMeteredKey method

पहले सेट किए गए लाइसेंस को हटाता है।

```csharp
public void ResetMeteredKey()
```

## उदाहरण

दिखाता है कि Aspose.Tasks के साथ <see cref=\"Aspose.Tasks.Metered\" /> लाइसेंस प्रकार का उपयोग कैसे करें।

```csharp
// आइए मीटर लाइसेंस का उपयोग करें (देखें https://purchase.aspose.com/faqs/licensing/metered)
// मीटर लाइसेंस सेट करें
var metered = new Metered();
metered.SetMeteredKey("<public key>", "<private key>");

var project = new Project(DataDir + "Project2.mpp");
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// ...
// परियोजना के साथ काम करें...
// ...

// हम वर्तमान क्रेडिट और बाइट्स की खपत प्राप्त कर सकते हैं।

try
{
    Console.WriteLine("Credits spent: {0}", Metered.GetConsumptionCredit());
    Console.WriteLine("Bytes consumed: {0}", Metered.GetConsumptionQuantity());
}
catch (WebException)
{
    // अपवाद लॉग करें
}

// हाल ही में उपयोगकर्ता मीटर को रीसेट कर सकता है और बाइट्स की गिनती रोक सकता है
metered.ResetMeteredKey();
```

### संबंधित देखें

* class [Metered](../)
* namespace [Aspose.Tasks](../../metered/)
* assembly [Aspose.Tasks](../../../)


