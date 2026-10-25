---
title: "क्लास Metered"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Metered क्लास। मीटर की सेट करने के लिए मेथड्स प्रदान करता है"
type: docs
weight: 1020
url: /hi/net/aspose.tasks/metered/
---
## Metered class

मीटरड कुंजी सेट करने के लिए मेथड्स प्रदान करता है।

```csharp
public class Metered
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Metered](metered/)() | डिफ़ॉल्ट कन्स्ट्रक्टर। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [IsLicensed](../../aspose.tasks/metered/islicensed/)() | जाँचता है कि उत्पाद मीटर लाइसेंस का उपयोग करके सफलतापूर्वक लाइसेंस प्राप्त है या नहीं। |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | पहले सेट किए गए लाइसेंस को हटाता है। |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | मीटर सार्वजनिक और निजी कुंजियों को सेट करता है। |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | उपभोग क्रेडिट प्राप्त करता है। |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | उपभोग फ़ाइल आकार प्राप्त करता है। |

## उदाहरण

इस उदाहरण में, मीटर सार्वजनिक और निजी कुंजी सेट करने का प्रयास किया जाएगा।

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

घटक जार फ़ाइल:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


