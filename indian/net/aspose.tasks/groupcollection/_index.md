---
title: "क्लास GroupCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.GroupCollection क्लास। Group ऑब्जेक्ट्स की सूची रखता है। ICollectionGroup इंटरफ़ेस को इम्प्लीमेंट करता है।"
type: docs
weight: 780
url: /hi/net/aspose.tasks/groupcollection/
---
## GroupCollection class

[`Group`](../group/) ऑब्जेक्ट्स की सूची रखता है। ICollection&lt;Group&gt; इंटरफ़ेस को इम्प्लीमेंट करता है।

```csharp
public class GroupCollection : ICollection<Group>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/groupcollection/count/) { get; } | इस संग्रह में मौजूद तत्वों की संख्या प्राप्त करता है। |
| [IsReadOnly](../../aspose.tasks/groupcollection/isreadonly/) { get; } | यह दर्शाने वाला मान प्राप्त करता है कि यह संग्रह केवल-पढ़ने योग्य है या नहीं। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/groupcollection/add/)(Group) | निर्दिष्ट आइटम को इस संग्रह में जोड़ता है। |
| [Clear](../../aspose.tasks/groupcollection/clear/)() | इस संग्रह से सभी आइटम हटाता है। |
| [Contains](../../aspose.tasks/groupcollection/contains/)(Group) | यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है; अन्यथा false। |
| [CopyTo](../../aspose.tasks/groupcollection/copyto/)(Group[], int) | निर्दिष्ट एरे सूचकांक से शुरू करके इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है। |
| [GetEnumerator](../../aspose.tasks/groupcollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [Remove](../../aspose.tasks/groupcollection/remove/)(Group) | इस संग्रह से विशिष्ट वस्तु की पहली घटना को हटाता है। |
| [ToList](../../aspose.tasks/groupcollection/tolist/)() | एक ग्रुप कलेक्शन को [`Group`](../group/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |

## उदाहरण

दिखाता है कि ग्रुप्स के कलेक्शन के साथ कैसे काम करें।

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

// टास्क ग्रुप्स पर इटरेट करें
Console.WriteLine("Print task groups of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Group Count: " + project.TaskGroups.Count);
foreach (var group in project.TaskGroups)
{
    Console.WriteLine("Name: " + group.Name);
    Console.WriteLine("Show In Menu: " + group.ShowInMenu);
    Console.WriteLine();
}

// रिसोर्स ग्रुप्स पर इटरेट करें
Console.WriteLine("Project resource group count: " + project.ResourceGroups.Count);
foreach (var group in project.ResourceGroups)
{
    Console.WriteLine("Resource group Name: " + group.Name);
    Console.WriteLine("Resource group ShowInMenu" + group.ShowInMenu);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// दूसरे प्रोजेक्ट के ग्रुप्स को साफ़ करें
otherProject.TaskGroups.Clear();

// ग्रुप्स को दूसरे प्रोजेक्ट में कॉपी करें
var groups = new Group[project.TaskGroups.Count];
project.TaskGroups.CopyTo(groups, 0);

foreach (var group in groups)
{
    otherProject.TaskGroups.Add(group);
}

// कस्टम टास्क ग्रुप जोड़ें
var customGroup = new Group
{
    Name = "Custom Group",
    ShowInMenu = true
};

if (!otherProject.TaskGroups.Contains(customGroup))
{
    if (!otherProject.TaskGroups.IsReadOnly)
    {
        otherProject.TaskGroups.Add(customGroup);
    }
}

// सभी ग्रुप्स हटाएँ
List<Group> groupsToDelete = otherProject.TaskGroups.ToList();
foreach (var group in groupsToDelete)
{
    otherProject.TaskGroups.Remove(group);
}
```

### संबंधित देखें

* class [Group](../group/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


