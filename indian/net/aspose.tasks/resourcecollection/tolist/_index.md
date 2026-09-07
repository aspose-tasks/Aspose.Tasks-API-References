---
title: "ResourceCollection.ToList"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceCollection method. ResourceCollection ऑब्जेक्ट को Resource ऑब्जेक्ट की सूची में परिवर्तित करता है"
type: docs
weight: 100
url: /hi/net/aspose.tasks/resourcecollection/tolist/
---
## ResourceCollection.ToList method

ResourceCollection ऑब्जेक्ट को [`Resource`](../../resource/) ऑब्जेक्ट की सूची में परिवर्तित करता है।

```csharp
public List<Resource> ToList()
```

### रिटर्न वैल्यू

[`Resource`](../../resource/) ऑब्जेक्ट की सूची।

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


