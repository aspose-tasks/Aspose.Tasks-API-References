---
title: "LoadOptions.Password"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "LoadOptions प्रॉपर्टी। एक प्रोटेक्शन पासवर्ड प्राप्त करता है या सेट करता है।"
type: docs
weight: 50
url: /hi/net/aspose.tasks/loadoptions/password/
---
## LoadOptions.Password property

प्रोटेक्शन पासवर्ड को प्राप्त करता है या सेट करता है।

```csharp
public string Password { get; set; }
```

## उदाहरण

<see cref=\"Aspose.Tasks.LoadOptions\"/> इंस्टेंस का उपयोग करके पासवर्ड-प्रोटेक्टेड प्रोजेक्ट को लोड करने का तरीका दिखाता है।

```csharp
using (var stream = new FileStream(DataDir + "PasswordProtectedProject.mpp", FileMode.Open))
{
    var options = new LoadOptions
    {
        Password = "password"
    };
    var project = new Project(stream, options);
    Console.WriteLine(project.Get(Prj.Name));
}
```

### संबंधित देखें

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


