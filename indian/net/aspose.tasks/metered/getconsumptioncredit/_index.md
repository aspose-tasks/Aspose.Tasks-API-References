---
title: "Metered.GetConsumptionCredit"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Metered मेथड। उपभोग क्रेडिट प्राप्त करता है।"
type: docs
weight: 50
url: /hi/net/aspose.tasks/metered/getconsumptioncredit/
---
## Metered.GetConsumptionCredit method

उपभोग क्रेडिट प्राप्त करता है।

```csharp
public static decimal GetConsumptionCredit()
```

### रिटर्न वैल्यू

उपभोग किए गए क्रेडिट पॉइंट्स की संख्या लौटाता है।

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


