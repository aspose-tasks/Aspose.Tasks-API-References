---
title: "ProjectView.GetDefaultAssignmentView"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ProjectView मेथड। इसमें Uid, टास्क नाम, रिसोर्स नाम, कार्य और अवधि असाइनमेंट कॉलम शामिल हैं"
type: docs
weight: 20
url: /hi/net/aspose.tasks.visualization/projectview/getdefaultassignmentview/
---
## ProjectView.GetDefaultAssignmentView method

Uid, कार्य नाम, संसाधन नाम, कार्य और अवधि असाइनमेंट कॉलम शामिल करता है।

```csharp
public static ProjectView GetDefaultAssignmentView()
```

### रिटर्न वैल्यू

एक दृश्य जिसमें [`AssignmentViewColumn`](../../assignmentviewcolumn/) की सूची शामिल है।

## उदाहरण

दिखाता है कि असाइनमेंट व्यू के साथ प्रोजेक्ट को कैसे सहेजें।

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultAssignmentView()
};

project.Save(OutDir + "WorkWithProjectView_AssignmentView_out.pdf", options);
```

### संबंधित देखें

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


