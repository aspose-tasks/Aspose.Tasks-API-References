---
title: "CopyToOptions.CopyToOptions"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "CopyToOptions कन्स्ट्रक्टर। CopyToOptions क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है"
type: docs
weight: 10
url: /hi/net/aspose.tasks/copytooptions/copytooptions/
---
## CopyToOptions constructor

[`CopyToOptions`](../) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

```csharp
public CopyToOptions()
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


