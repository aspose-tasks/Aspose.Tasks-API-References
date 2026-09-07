---
title: "ResourceLeveler.LevelResources"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceLeveler मेथड। निर्दिष्ट लेवलिंग विकल्पों का उपयोग करके निर्दिष्ट संसाधनों के लिए कार्यों को लेवल करता है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks.leveling/resourceleveler/levelresources/
---
## ResourceLeveler.LevelResources method

निर्दिष्ट लेवलिंग विकल्पों का उपयोग करके निर्दिष्ट संसाधनों के लिए कार्यों को लेवल करता है।

```csharp
public static LevelingResult LevelResources(Project project, LevelingOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रोजेक्ट | Project | रिसोर्स लेवलिंग लागू करने के लिए प्रोजेक्ट। |
| विकल्प | LevelingOptions | विकल्प जो निर्धारित करता है कि संसाधनों को कैसे लेवल किया जाए। |

### रिटर्न वैल्यू

ऑब्जेक्ट जिसमें रिसोर्स लेवलिंग के परिणाम होते हैं।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | यदि पैरामीटर options null है। |

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [LevelingOptions](../../levelingoptions/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


