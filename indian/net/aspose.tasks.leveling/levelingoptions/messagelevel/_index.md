---
title: "LevelingOptions.MessageLevel"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "LevelingOptions प्रॉपर्टी। संसाधन लेवलिंग के दौरान Aspose.Tasks द्वारा उत्पन्न लॉग संदेशों के स्तर को प्राप्त करता है या सेट करता है"
type: docs
weight: 60
url: /hi/net/aspose.tasks.leveling/levelingoptions/messagelevel/
---
## LevelingOptions.MessageLevel property

Aspose.Tasks द्वारा संसाधन लेवलिंग के दौरान उत्पन्न लॉग संदेशों के स्तर को प्राप्त करता है या सेट करता है।

```csharp
public MessageLevel MessageLevel { get; set; }
```

## उदाहरण

दिखाता है कि विशिष्ट संसाधन को कैसे लेवल किया जाए, लेवलिंग विकल्पों को अनुकूलित किया जाए और लेवलिंग एल्गोरिदम संदेशों की जांच की जाए।

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingOptions = new LevelingOptions();
levelingOptions.StartDate = new DateTime(2013, 3, 10);
levelingOptions.FinishDate = new DateTime(2013, 4, 30);
levelingOptions.Resources = new List<Resource> { project.Resources.GetById(7) };
levelingOptions.MessageLevel = MessageLevel.Information;
levelingOptions.MessageHandler = new LevelingMessageHandler();

ResourceLeveler.LevelResources(project, levelingOptions);
```

### संबंधित देखें

* enum [MessageLevel](../../../aspose.tasks/messagelevel/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


