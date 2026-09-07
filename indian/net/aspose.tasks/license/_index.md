---
title: "क्लास License"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.License क्लास। घटक को लाइसेंस करने के लिए मेथड्स प्रदान करती है"
type: docs
weight: 980
url: /hi/net/aspose.tasks/license/
---
## License class

घटक को लाइसेंस करने के लिए मेथड्स प्रदान करता है।

```csharp
public sealed class License
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [License](license/)() | `License` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense)(Stream) | घटक को लाइसेंस करता है। |
| [SetLicense](../../aspose.tasks/license/setlicense/#setlicense_1)(string) | घटक को लाइसेंस करता है। |

## उदाहरण

इस उदाहरण में, घटक वाले फ़ोल्डर, कॉलिंग असेंबली वाले फ़ोल्डर, एंट्री असेंबली वाले फ़ोल्डर और फिर कॉलिंग असेंबली के एम्बेडेड रिसोर्सेज़ में MyLicense.lic नाम की लाइसेंस फ़ाइल खोजने का प्रयास किया जाएगा।

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

घटक जार फ़ाइल:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

दिखाता है कि Aspose.Tasks का लाइसेंस कैसे लागू किया जाए।

```csharp
var license = new License();
license.SetLicense("Aspose.Tasks.lic");
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


