---
title: "Enum WorkGroupType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.WorkGroupType enum. एक कार्यसमूह के प्रकार को निर्दिष्ट करता है"
type: docs
weight: 3620
url: /hi/net/aspose.tasks/workgrouptype/
---
## WorkGroupType enumeration

वर्कग्रुप के प्रकार को निर्दिष्ट करता है।

```csharp
public enum WorkGroupType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Default | `0` | डिफ़ॉल्ट कार्यसमूह प्रकार को दर्शाता है। |
| None | `1` | कोई कार्यसमूह प्रकार नहीं को दर्शाता है। |
| Email | `2` | ईमेल कार्यसमूह प्रकार को दर्शाता है। |
| Web | `3` | वेब कार्यसमूह प्रकार को दर्शाता है। |

## उदाहरण

दिखाता है कि संसाधन का कार्यसमूह कैसे सेट करें।

```csharp
var project = new Project();

// ...
var resource = project.Resources.Add("Resource");
resource.Set(Rsc.Workgroup, WorkGroupType.Web);

// ...
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


