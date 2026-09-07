---
title: "क्लास PrimaveraReadOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.PrimaveraReadOptions क्लास। Primavera Xml या Primavera Xer फ़ाइलों को पढ़ते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।"
type: docs
weight: 1370
url: /hi/net/aspose.tasks/primaverareadoptions/
---
## PrimaveraReadOptions class

Primavera XML या Primavera XER फ़ाइलें पढ़ते समय अतिरिक्त विकल्प निर्दिष्ट करने की अनुमति देता है।

```csharp
public class PrimaveraReadOptions
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [PrimaveraReadOptions](primaverareadoptions/)() | `PrimaveraReadOptions` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [PreserveUids](../../aspose.tasks/primaverareadoptions/preserveuids/) { get; set; } | एक फ़्लैग प्राप्त करता है या सेट करता है जो यह निर्दिष्ट करता है कि इकाइयों के मूल अद्वितीय पहचानकर्ता संरक्षित किए जाने चाहिए या नहीं। |
| [ProjectUid](../../aspose.tasks/primaverareadoptions/projectuid/) { get; set; } | एक फ़ाइल जिसमें कई प्रोजेक्ट हैं, से पढ़ने के लिए प्रोजेक्ट का UID प्राप्त करता है या सेट करता है। |
| [ReadBaselineProjects](../../aspose.tasks/primaverareadoptions/readbaselineprojects/) { get; set; } | एक फ़्लैग प्राप्त करता है या सेट करता है जो यह निर्दिष्ट करता है कि बेसलाइन प्रोजेक्ट लोड किए जाने चाहिए या नहीं। डिफ़ॉल्ट मान true है। |
| [UndefinedConstraintHandlingBehavior](../../aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/) { get; set; } | XER फ़ॉर्मेट से पढ़े गए अनिर्धारित प्रतिबंधों वाले टास्क को प्रोसेस करने के लिए उपयोग किए जाने वाले व्यवहार को निर्दिष्ट करता है। |

## उदाहरण

दिखाता है कि कई प्रोजेक्ट्स वाली Primavera XML या Primavera XER फ़ाइल से प्रोजेक्ट कैसे पढ़ें।

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// विशेष UID वाला प्रोजेक्ट लौटाता है।
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


