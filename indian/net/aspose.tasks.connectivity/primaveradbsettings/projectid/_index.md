---
title: "PrimaveraDbSettings.ProjectId"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "PrimaveraDbSettings प्रॉपर्टी। पढ़ने के लिए प्रोजेक्ट की आईडी प्राप्त करता है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks.connectivity/primaveradbsettings/projectid/
---
## PrimaveraDbSettings.ProjectId property

पढ़ने के लिए प्रोजेक्ट का आईडी प्राप्त करता है।

```csharp
public int ProjectId { get; }
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

* class [PrimaveraDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../primaveradbsettings/)
* assembly [Aspose.Tasks](../../../)


