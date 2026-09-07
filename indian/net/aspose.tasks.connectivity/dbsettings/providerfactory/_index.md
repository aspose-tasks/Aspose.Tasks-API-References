---
title: "DbSettings.ProviderFactory"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "DbSettings प्रॉपर्टी। एक DbProviderFactory का इंस्टेंस प्राप्त करता है या सेट करता है जिसका उपयोग DB से कनेक्ट करने के लिए किया जाता है। यदि दोनों ProviderFactory और ProviderInvariantName सेट हैं तो ProviderFactory को प्राथमिकता मिलती है। डिफ़ॉल्ट मान null है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks.connectivity/dbsettings/providerfactory/
---
## DbSettings.ProviderFactory property

DB से कनेक्ट करने के लिए उपयोग की जाने वाली DbProviderFactory का एक इंस्टेंस प्राप्त करता है या सेट करता है। यदि दोनों ProviderFactory और ProviderInvariantName सेट हैं, तो ProviderFactory को प्राथमिकता मिलती है। डिफ़ॉल्ट मान null है।

```csharp
public DbProviderFactory ProviderFactory { get; set; }
```

## उदाहरण

Primavera डेटाबेस से प्रोजेक्ट इम्पोर्ट करने का तरीका दिखाता है।

```csharp
// कनेक्शन स्ट्रिंग और प्रोजेक्ट आईडी के साथ PrimaveraDbSettings क्लास का एक नया इंस्टेंस इनिशियलाइज़ करें
var settings = new PrimaveraDbSettings(GetConnectionString(), 4502);
settings.ProviderFactory = SqliteFactory.Instance;

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// UID = 4502 के साथ प्रोजेक्ट पढ़ें
var project = new Project(settings);
Console.WriteLine(project.Uid);
Console.WriteLine(project.Name);
Console.WriteLine(project.PrimaveraProperties.ShortName);
```

### संबंधित देखें

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


