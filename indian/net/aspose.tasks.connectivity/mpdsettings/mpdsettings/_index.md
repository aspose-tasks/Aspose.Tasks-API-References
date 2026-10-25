---
title: "MpdSettings.MpdSettings"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "MpdSettings कंस्ट्रक्टर। MpdSettings क्लास का एक नया उदाहरण इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks.connectivity/mpdsettings/mpdsettings/
---
## MpdSettings constructor

[`MpdSettings`](../) क्लास का एक नया उदाहरण इनिशियलाइज़ करता है।

```csharp
public MpdSettings(string connectionString, int projectId)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| connectionString | स्ट्रिंग | निर्दिष्ट कनेक्शन स्ट्रिंग। |
| projectId | Int32 | पढ़ने के लिए प्रोजेक्ट का निर्दिष्ट ID। |

## उदाहरण

दिखाता है कि MPD फ़ाइल से प्रोजेक्ट कैसे पढ़ा जाए।

```csharp
DbSettings settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### संबंधित देखें

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


