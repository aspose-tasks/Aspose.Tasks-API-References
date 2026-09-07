---
title: "FieldHelper.GetDefaultTaskFieldTitle"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "FieldHelper मेथड। विशिष्ट टास्क फ़ील्ड का डिफ़ॉल्ट शीर्षक लौटाता है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks.util/fieldhelper/getdefaulttaskfieldtitle/
---
## FieldHelper.GetDefaultTaskFieldTitle method

विशिष्ट टास्क फ़ील्ड का डिफ़ॉल्ट शीर्षक लौटाता है।

```csharp
public static string GetDefaultTaskFieldTitle(TaskKey taskKey)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| taskKey | TaskKey | डिफ़ॉल्ट शीर्षक प्राप्त करने के लिए टास्क फ़ील्ड। |

### रिटर्न वैल्यू

यदि फ़ील्ड MS Project के व्यू में प्रदर्शित हो सकता है तो विशिष्ट टास्क फ़ील्ड का डिफ़ॉल्ट शीर्षक, अन्यथा null।

## उदाहरण

विशिष्ट टास्क फ़ील्ड के लिए डिफ़ॉल्ट फ़ील्ड शीर्षक कैसे प्राप्त करें, यह दर्शाता है।

```csharp
Console.WriteLine("Title for Tsk.ActualCost: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.ActualCost.KeyType));
Console.WriteLine("Title for Tsk.PercentWorkComplete: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.PercentWorkComplete.KeyType));
```

### संबंधित देखें

* enum [TaskKey](../../../aspose.tasks/taskkey/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


