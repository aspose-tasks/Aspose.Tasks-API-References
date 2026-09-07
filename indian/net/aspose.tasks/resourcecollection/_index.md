---
title: "क्लास ResourceCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ResourceCollection क्लास। Resource ऑब्जेक्ट्स का संग्रह दर्शाता है"
type: docs
weight: 1770
url: /hi/net/aspose.tasks/resourcecollection/
---
## ResourceCollection class

[`Resource`](../resource/) ऑब्जेक्ट्स का संग्रह दर्शाता है।

```csharp
public class ResourceCollection : IList<Resource>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/resourcecollection/count/) { get; } | ResourceCollection में सम्मिलित तत्वों की संख्या प्राप्त करता है। केवल-पढ़ने योग्य Int32। |
| [Item](../../aspose.tasks/resourcecollection/item/) { get; set; } | निर्दिष्ट इंडेक्स पर तत्व लौटाता है। |
| [ParentProject](../../aspose.tasks/resourcecollection/parentproject/) { get; } | ResourceCollection ऑब्जेक्ट के पैरेंट प्रोजेक्ट को प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/resourcecollection/add/#add)() | प्रोजेक्ट संसाधन संग्रह के अंतिम स्थान पर नया संसाधन जोड़ता है। |
| [Add](../../aspose.tasks/resourcecollection/add/#add_1)(string) | प्रोजेक्ट संसाधन संग्रह के अंतिम स्थान पर नया संसाधन जोड़ता है। |
| [Add](../../aspose.tasks/resourcecollection/add/#add_2)(string, int) | प्रोजेक्ट संसाधन संग्रह के निर्दिष्ट स्थान पर नया संसाधन जोड़ता है। |
| [Clear](../../aspose.tasks/resourcecollection/clear/)() | सीधे क्लियरिंग का समर्थन नहीं है, यह मेथड केवल NotSupportedException फेंकता है। |
| [GetById](../../aspose.tasks/resourcecollection/getbyid/)(int) | निर्दिष्ट id वाला संसाधन लौटाता है। |
| [GetByUid](../../aspose.tasks/resourcecollection/getbyuid/)(int) | निर्दिष्ट Uid वाला संसाधन लौटाता है। |
| [GetEnumerator](../../aspose.tasks/resourcecollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [Remove](../../aspose.tasks/resourcecollection/remove/)(Resource) | यह ICollection की Remove मेथड का स्टब इम्प्लीमेंटेशन है, जो केवल NotSupportedException फेंकता है। |
| [ToList](../../aspose.tasks/resourcecollection/tolist/)() | ResourceCollection ऑब्जेक्ट को [`Resource`](../resource/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |

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

* class [Resource](../resource/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


