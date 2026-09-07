---
title: "GroupCollection.CopyTo"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GroupCollection मेथड। इस संग्रह के तत्वों को निर्दिष्ट एरे में निर्दिष्ट एरे इंडेक्स से शुरू करके कॉपी करता है।"
type: docs
weight: 60
url: /hi/net/aspose.tasks/groupcollection/copyto/
---
## GroupCollection.CopyTo method

निर्दिष्ट एरे सूचकांक से शुरू करके इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है।

```csharp
public void CopyTo(Group[] array, int arrayIndex)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| एरे | Group[] | तत्वों को कॉपी करने के लिए निर्दिष्ट एक-आयामी एरे |
| arrayIndex | Int32 | निर्दिष्ट एरे का शून्य-आधारित इंडेक्स जहाँ से कॉपी शुरू होती है। |

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

* class [Group](../../group/)
* class [GroupCollection](../)
* namespace [Aspose.Tasks](../../groupcollection/)
* assembly [Aspose.Tasks](../../../)


