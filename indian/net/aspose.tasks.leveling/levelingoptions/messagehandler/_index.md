---
title: "LevelingOptions.MessageHandler"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "LevelingOptions प्रॉपर्टी। संदेश हैंडलर कॉलबैक को प्राप्त करता है या सेट करता है जिसका उपयोग संसाधन लेवलिंग के दौरान Aspose.Tasks द्वारा उत्पन्न लॉग संदेशों को इंटरसेप्ट करने के लिए किया जा सकता है"
type: docs
weight: 50
url: /hi/net/aspose.tasks.leveling/levelingoptions/messagehandler/
---
## LevelingOptions.MessageHandler property

एक संदेश हैंडलर कॉलबैक प्राप्त करता है या सेट करता है जिसका उपयोग Aspose.Tasks द्वारा संसाधन लेवलिंग के दौरान उत्पन्न लॉग संदेशों को इंटरसेप्ट करने के लिए किया जा सकता है।

```csharp
public IMessageHandler MessageHandler { get; set; }
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

* interface [IMessageHandler](../../../aspose.tasks/imessagehandler/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


