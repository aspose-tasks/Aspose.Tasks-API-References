---
title: "MpdSettings.ProjectId"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "MpdSettings प्रॉपर्टी। पढ़ने के लिए प्रोजेक्ट का ID प्राप्त करता है"
type: docs
weight: 20
url: /hi/net/aspose.tasks.connectivity/mpdsettings/projectid/
---
## MpdSettings.ProjectId property

पढ़ने के लिए प्रोजेक्ट का आईडी प्राप्त करता है।

```csharp
public int ProjectId { get; }
```

## उदाहरण

डेटाबेस से प्रोजेक्ट इम्पोर्ट को नियंत्रित करने के लिए MPD सेटिंग्स का उपयोग कैसे करें, यह दिखाता है।

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### संबंधित देखें

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


