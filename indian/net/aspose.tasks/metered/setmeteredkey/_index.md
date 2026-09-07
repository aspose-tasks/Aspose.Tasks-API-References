---
title: "Metered.SetMeteredKey"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Metered मेथड। मीटरड सार्वजनिक और निजी कुंजियों को सेट करता है"
type: docs
weight: 40
url: /hi/net/aspose.tasks/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

मीटर सार्वजनिक और निजी कुंजियों को सेट करता है।

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| publicKey | स्ट्रिंग | सार्वजनिक कुंजी। |
| privateKey | स्ट्रिंग | निजी कुंजी। |

## टिप्पणियाँ

यदि आप मीटरड लाइसेंस खरीदते हैं, तो इस API को एप्लिकेशन स्टार्टअप पर कॉल किया जाना चाहिए, सामान्यतः यह पर्याप्त है। हालांकि, यदि मीटरड 24 घंटे की अवधि में उपभोग डेटा अपलोड करने में विफल रहता है, तो लाइसेंस को मूल्यांकन स्थिति में सेट कर दिया जाएगा। ऐसे मामले से बचने के लिए, आपको नियमित रूप से लाइसेंस स्थिति की जाँच करनी चाहिए। यदि यह मूल्यांकन स्थिति है, तो इस API को फिर से कॉल करें।

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


