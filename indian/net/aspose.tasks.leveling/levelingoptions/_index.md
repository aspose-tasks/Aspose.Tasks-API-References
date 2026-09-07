---
title: "क्लास LevelingOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Leveling.LevelingOptions क्लास। संसाधन लेवलिंग के पैरामीटर निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 940
url: /hi/net/aspose.tasks.leveling/levelingoptions/
---
## LevelingOptions class

रिसोर्स लेवलिंग के पैरामीटर निर्दिष्ट करने की अनुमति देता है।

```csharp
public sealed class LevelingOptions
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [LevelingOptions](levelingoptions/)() | `LevelingOptions` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [CancellationToken](../../aspose.tasks.leveling/levelingoptions/cancellationtoken/) { get; set; } | एक टोकन प्राप्त करता है या सेट करता है जिसका उपयोग प्रोजेक्ट लेवलिंग ऑपरेशन को रद्द करने के लिए किया जा सकता है। |
| [FinishDate](../../aspose.tasks.leveling/levelingoptions/finishdate/) { get; set; } | लेवलिंग अवधि की समाप्ति तिथि प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान प्रोजेक्ट की समाप्ति तिथि है। |
| [LevelingOrder](../../aspose.tasks.leveling/levelingoptions/levelingorder/) { get; set; } | लेवलिंग एल्गोरिद्म द्वारा अधिक आवंटन वाले कार्यों को विलंबित करने के क्रम को प्राप्त करता है। ओवरएलोकेशन का कारण बनने वाले कार्यों और जिन्हें विलंबित किया जा सकता है, निर्धारित करने के बाद, निर्दिष्ट क्रम का उपयोग किया जाता है कि कौन सा कार्य पहले विलंबित होना चाहिए। |
| [MessageHandler](../../aspose.tasks.leveling/levelingoptions/messagehandler/) { get; set; } | एक संदेश हैंडलर कॉलबैक प्राप्त करता है या सेट करता है जिसका उपयोग Aspose.Tasks द्वारा संसाधन लेवलिंग के दौरान उत्पन्न लॉग संदेशों को इंटरसेप्ट करने के लिए किया जा सकता है। |
| [MessageLevel](../../aspose.tasks.leveling/levelingoptions/messagelevel/) { get; set; } | Aspose.Tasks द्वारा संसाधन लेवलिंग के दौरान उत्पन्न लॉग संदेशों के स्तर को प्राप्त करता है या सेट करता है। |
| [Resources](../../aspose.tasks.leveling/levelingoptions/resources/) { get; set; } | उन संसाधनों की सूची प्राप्त करता है या सेट करता है जिन्हें लेवल किया जाएगा। यदि null सेट किया जाता है, तो सभी प्रोजेक्ट संसाधनों को लेवल किया जाएगा। |
| [StartDate](../../aspose.tasks.leveling/levelingoptions/startdate/) { get; set; } | लेवलिंग अवधि की प्रारंभ तिथि प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान प्रोजेक्ट की प्रारंभ तिथि है। |

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

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


