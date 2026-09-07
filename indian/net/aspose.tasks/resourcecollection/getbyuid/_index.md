---
title: "ResourceCollection.GetByUid"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceCollection मेथड। निर्दिष्ट Uid के साथ एक संसाधन लौटाता है।"
type: docs
weight: 70
url: /hi/net/aspose.tasks/resourcecollection/getbyuid/
---
## ResourceCollection.GetByUid method

निर्दिष्ट Uid वाला संसाधन लौटाता है।

```csharp
public Resource GetByUid(int uid)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| uid | Int32 | निर्दिष्ट uid। |

### रिटर्न वैल्यू

यदि मौजूद हो तो निर्दिष्ट uid वाला संसाधन; अन्यथा, null।

## टिप्पणियाँ

O(1) जटिलता।

## उदाहरण

संसाधन संग्रहों के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// खाली संसाधन जोड़ें
var resource = project.Resources.Add();
resource.Set(Rsc.Type, ResourceType.Work);

// नाम के साथ संसाधन जोड़ें
var developer = project.Resources.Add("Developer");
developer.Set(Rsc.Type, ResourceType.Work);

// निर्दिष्ट ID वाले संसाधन से पहले संसाधन जोड़ें
var manager = project.Resources.Add("Manager", developer.Get(Rsc.Id));
manager.Set(Rsc.Type, ResourceType.Work);

var devResource = project.Resources.GetById(4);
devResource.Set(Rsc.Code, "12345");

var manResource = project.Resources.GetByUid(4);
manResource.Set(Rsc.Code, "54321");

// id द्वारा संसाधन प्राप्त करें
project.Resources.GetById(1);

Console.WriteLine("Print the resources of " + project.Resources.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Count of resources: " + project.Resources.Count);
foreach (var rsc in project.Resources)
{
    Console.WriteLine("Resource Name: " + rsc.Get(Rsc.Name));
}

Console.WriteLine();

// संसाधन संग्रह Clear ऑपरेशन का समर्थन नहीं करता है
// project.Resources.Clear();
// इसके बजाय अगला कोड नमूना उपयोग करें
List<Resource> list = project.Resources.ToList();
foreach (var rsc in list)
{
    rsc.Delete();
}
```

### संबंधित देखें

* class [Resource](../../resource/)
* class [ResourceCollection](../)
* namespace [Aspose.Tasks](../../resourcecollection/)
* assembly [Aspose.Tasks](../../../)


