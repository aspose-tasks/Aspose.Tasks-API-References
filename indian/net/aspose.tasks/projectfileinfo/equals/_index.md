---
title: "ProjectFileInfo.Equals"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectFileInfo मेथड। एक मान लौटाता है जो दर्शाता है कि यह इंस्टेंस निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं"
type: docs
weight: 50
url: /hi/net/aspose.tasks/projectfileinfo/equals/
---
## Equals(ProjectFileInfo) {#equals}

यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public bool Equals(ProjectFileInfo other)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| अन्य | ProjectFileInfo | निर्दिष्ट ऑब्जेक्ट जो इस इंस्टेंस से तुलना करने के लिए है। |

### रिटर्न वैल्यू

यदि निर्दिष्ट ProjectFileInfo और यह इंस्टेंस समान फ़ाइल फ़ॉर्मेट और एप्लिकेशन जानकारी रखते हैं तो true लौटाता है।

## उदाहरण

प्रोजेक्ट फ़ाइल की जानकारी पढ़ने का तरीका दर्शाता है।

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### संबंधित देखें

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं।

```csharp
public override bool Equals(object obj)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| obj | ऑब्जेक्ट | निर्दिष्ट ऑब्जेक्ट जो इस इंस्टेंस से तुलना करने के लिए है। |

### रिटर्न वैल्यू

यदि निर्दिष्ट ProjectFileInfo और यह इंस्टेंस समान फ़ाइल फ़ॉर्मेट और एप्लिकेशन जानकारी रखते हैं तो true लौटाता है।

## उदाहरण

प्रोजेक्ट फ़ाइल की जानकारी पढ़ने का तरीका दर्शाता है।

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### संबंधित देखें

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


