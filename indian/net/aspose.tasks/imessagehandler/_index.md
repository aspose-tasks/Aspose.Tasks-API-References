---
title: "इंटरफ़ेस IMessageHandler"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.IMessageHandler इंटरफ़ेस। रिसोर्स लेवलिंग के परिणामों के लिए एक कॉलबैक को दर्शाता है"
type: docs
weight: 880
url: /hi/net/aspose.tasks/imessagehandler/
---
## IMessageHandler interface

संसाधन लेवलिंग के परिणामों के लिए कॉलबैक का प्रतिनिधित्व करता है।

```csharp
public interface IMessageHandler
```

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Message](../../aspose.tasks/imessagehandler/message/)(MessageLevel, string) | Aspose.Tasks जब संदेश आउटपुट करता है तो इस मेथड को कॉल करता है। |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


