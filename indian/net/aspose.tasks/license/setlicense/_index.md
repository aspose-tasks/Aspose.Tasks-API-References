---
title: "License.SetLicense"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "License मेथड। घटक को लाइसेंस देता है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

घटक को लाइसेंस करता है।

```csharp
public void SetLicense(string licenseName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| licenseName | स्ट्रिंग | पूरा या छोटा फ़ाइल नाम या एम्बेडेड रिसोर्स का नाम हो सकता है। मूल्यांकन मोड में स्विच करने के लिए खाली स्ट्रिंग उपयोग करें। |

## टिप्पणियाँ

लाइसेंस को निम्नलिखित स्थानों में खोजने का प्रयास करता है:

1. स्पष्ट पथ।

2. वह फ़ोल्डर जिसमें Aspose घटक असेंबली है।

3. वह फ़ोल्डर जिसमें क्लाइंट की कॉलिंग असेंबली है।

4. वह फ़ोल्डर जिसमें एंट्री (स्टार्टअप) असेंबली है।

5. क्लाइंट की कॉलिंग असेंबली में एम्बेडेड रिसोर्स।

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. स्पष्ट पथ।

2. क्लाइंट की कॉलिंग असेंबली में एम्बेडेड रिसोर्स।

2. वह फ़ोल्डर जिसमें Aspose घटक JAR फ़ाइल है।

3. वह फ़ोल्डर जिसमें क्लाइंट की कॉलिंग JAR फ़ाइल है।

## उदाहरण

इस उदाहरण में, घटक वाले फ़ोल्डर, कॉलिंग असेंबली वाले फ़ोल्डर, एंट्री असेंबली वाले फ़ोल्डर और फिर कॉलिंग असेंबली के एम्बेडेड रिसोर्सेज़ में MyLicense.lic नाम की लाइसेंस फ़ाइल खोजने का प्रयास किया जाएगा।

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");
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

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)

---

## SetLicense(Stream) {#setlicense}

घटक को लाइसेंस करता है।

```csharp
public void SetLicense(Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | स्ट्रीम | एक स्ट्रीम जिसमें लाइसेंस शामिल है। |

## टिप्पणियाँ

इस मेथड का उपयोग करके स्ट्रीम से लाइसेंस लोड करें।

## उदाहरण

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)

License license = new License();
license.setLicense(myStream);
```

दिखाता है कि कैसे Aspose.Tasks का लाइसेंस लागू किया जाए जो <see cref=\"System.IO.FileStream\" /> से पढ़ा गया है।

```csharp
var license = new License();
using (var stream = new FileStream("Aspose.Tasks.lic", FileMode.Open))
{
    license.SetLicense(stream);
}
```

### संबंधित देखें

* class [License](../)
* namespace [Aspose.Tasks](../../license/)
* assembly [Aspose.Tasks](../../../)


