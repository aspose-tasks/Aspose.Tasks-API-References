---
title: "क्लास CopyToOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.CopyToOptions क्लास। प्रोजेक्ट डेटा कॉपी करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है"
type: docs
weight: 340
url: /hi/net/aspose.tasks/copytooptions/
---
## CopyToOptions class

प्रोजेक्ट डेटा कॉपी करते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।

```csharp
public class CopyToOptions
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [CopyToOptions](copytooptions/)() | `CopyToOptions` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [CopyViewData](../../aspose.tasks/copytooptions/copyviewdata/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि प्रोजेक्ट डेटा कॉपी करते समय व्यू डेटा कॉपी किया जाए या नहीं। डिफ़ॉल्ट मान true है। |

## उदाहरण

दिखाता है कि प्रोजेक्ट कॉपी विकल्पों का उपयोग कैसे करें।

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// सामान्य प्रोजेक्ट डेटा कॉपी करते समय व्यू डेटा की कॉपी को छोड़ें।
var copyToOptions = new CopyToOptions();
copyToOptions.CopyViewData = false;
project.CopyTo(mppProject, copyToOptions);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


