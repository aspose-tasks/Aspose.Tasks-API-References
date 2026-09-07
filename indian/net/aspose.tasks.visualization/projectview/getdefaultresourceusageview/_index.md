---
title: "ProjectView.GetDefaultResourceUsageView"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectView मेथड। इसमें Uid, नाम, प्रारंभ, समाप्ति और कार्य संसाधन कॉलम शामिल हैं"
type: docs
weight: 50
url: /hi/net/aspose.tasks.visualization/projectview/getdefaultresourceusageview/
---
## ProjectView.GetDefaultResourceUsageView method

Uid, name, start, finish और work resource कॉलम शामिल हैं।

```csharp
public static ProjectView GetDefaultResourceUsageView()
```

### रिटर्न वैल्यू

एक दृश्य जिसमें [`ResourceViewColumn`](../../resourceviewcolumn/) की सूची शामिल है।

## उदाहरण

दिखाता है कि संसाधन उपयोग दृश्य के साथ प्रोजेक्ट को कैसे सहेजें।

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceUsageView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceUsageView_out.pdf", options);
```

### संबंधित देखें

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


