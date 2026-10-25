---
title: "CopyToOptions.CopyViewData"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CopyToOptions प्रॉपर्टी। एक मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि प्रोजेक्ट डेटा कॉपी करते समय व्यू डेटा कॉपी किया जाए या नहीं। डिफ़ॉल्ट मान true है"
type: docs
weight: 20
url: /hi/net/aspose.tasks/copytooptions/copyviewdata/
---
## CopyToOptions.CopyViewData property

एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि प्रोजेक्ट डेटा कॉपी करते समय व्यू डेटा कॉपी किया जाए या नहीं। डिफ़ॉल्ट मान true है।

```csharp
public bool CopyViewData { get; set; }
```

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

* class [CopyToOptions](../)
* namespace [Aspose.Tasks](../../copytooptions/)
* assembly [Aspose.Tasks](../../../)


