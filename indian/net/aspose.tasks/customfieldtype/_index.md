---
title: "Enum CustomFieldType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.CustomFieldType enum. एक कस्टम फ़ील्ड के प्रकार को निर्दिष्ट करता है।"
type: docs
weight: 380
url: /hi/net/aspose.tasks/customfieldtype/
---
## CustomFieldType enumeration

कस्टम फ़ील्ड के प्रकार को निर्दिष्ट करता है।

```csharp
public enum CustomFieldType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Null | `0` | Null कस्टम फ़ील्ड प्रकार को दर्शाता है। |
| Cost | `1` | Cost कस्टम फ़ील्ड प्रकार को दर्शाता है। |
| Date | `2` | Date कस्टम फ़ील्ड प्रकार को दर्शाता है। |
| Duration | `3` | Duration कस्टम फ़ील्ड प्रकार को दर्शाता है। |
| Finish | `4` | Finish कस्टम फ़ील्ड प्रकार को दर्शाता है। |
| Flag | `5` | Flag कस्टम फ़ील्ड प्रकार को दर्शाता है। |
| Number | `6` | Number कस्टम फ़ील्ड प्रकार को दर्शाता है। |
| Start | `7` | Start कस्टम फ़ील्ड प्रकार को दर्शाता है। |
| Text | `8` | Text कस्टम फ़ील्ड प्रकार को दर्शाता है। |
| OutlineCode | `9` | Outline Code कस्टम फ़ील्ड प्रकार को दर्शाता है। |
| RBS | `10` | RBS (Resource Breakdown Structure) कस्टम फ़ील्ड प्रकार को दर्शाता है। |

## उदाहरण

दिखाता है कि कैसे उपयोग करें &lt;see cref=\"CustomFieldType\" /&gt; (CustomFieldType.Text).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text1,
    "MyText");
project.ExtendedAttributes.Add(definition);
// परिभाषाओं के साथ काम करें...
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


