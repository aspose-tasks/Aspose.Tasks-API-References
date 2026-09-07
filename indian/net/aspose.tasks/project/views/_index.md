---
title: "Project.Views"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। View ऑब्जेक्ट्स की सूची प्राप्त करता है।"
type: docs
weight: 1020
url: /hi/net/aspose.tasks/project/views/
---
## Project.Views property

[`View`](../../view/) ऑब्जेक्ट्स की सूची प्राप्त करता है।

```csharp
public ViewCollection Views { get; }
```

## उदाहरण

डिफ़ॉल्ट प्रोजेक्ट व्यू सेट करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project5.mpp");

View view = null;
foreach (var v in project.Views)
{
    if (v.Name == "&Gantt Chart")
    {
        view = v;
    }
}

// डिफ़ॉल्ट व्यू सेट करें
project.DefaultView = view;

project.Save(OutDir + @"SaveGantChartView_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### संबंधित देखें

* class [ViewCollection](../../viewcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


