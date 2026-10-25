---
title: "OleObjectCollection.Clear"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "OleObjectCollection विधि. संग्रह को साफ़ करता है। इन परिवर्तनों को स्थायी बनाने के लिए project.Save को new MPPSaveOptions  WriteViewData  true के साथ बुलाया जाना चाहिए।"
type: docs
weight: 10
url: /hi/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

संग्रह को साफ़ करता है। इन परिवर्तनों को स्थायी बनाने के लिए project.Save को नए MPPSaveOptions { WriteViewData = true; } के साथ बुलाया जाना चाहिए।

```csharp
public void Clear()
```

## उदाहरण

OLE ऑब्जेक्ट्स को साफ़ करने और इन परिवर्तनों को स्थायी बनाने का तरीका।

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

निर्दिष्ट प्रोजेक्ट से OLE ऑब्जेक्ट्स को हटाने का तरीका दिखाता है।

```csharp
[Test]
public void ClearOleObjects()
{
    var project = new Project(DataDir + "TaskImage2010.mpp");
    project.OleObjects.Clear();
    project.Save(OutDir + "ClearedProject.mpp");
}
```

### संबंधित देखें

* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


