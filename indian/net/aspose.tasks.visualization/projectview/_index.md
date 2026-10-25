---
title: "Class ProjectView"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.ProjectView class. प्रोजेक्ट व्यू क्लास।"
type: docs
weight: 3300
url: /hi/net/aspose.tasks.visualization/projectview/
---
## ProjectView class

प्रोजेक्ट का दृश्य वर्ग

```csharp
public class ProjectView
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [ProjectView](projectview/)(IEnumerable&lt;ViewColumn&gt;) | `ProjectView` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Columns](../../aspose.tasks.visualization/projectview/columns/) { get; } | प्रोजेक्ट व्यू कॉलम प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| static [GetDefaultAssignmentView](../../aspose.tasks.visualization/projectview/getdefaultassignmentview/)() | Uid, कार्य नाम, संसाधन नाम, कार्य और अवधि असाइनमेंट कॉलम शामिल करता है। |
| static [GetDefaultGanttChartView](../../aspose.tasks.visualization/projectview/getdefaultganttchartview/)() | id, संकेतक, नाम, अवधि, प्रारंभ और समाप्ति कार्य कॉलम शामिल करता है। |
| static [GetDefaultResourceSheetView](../../aspose.tasks.visualization/projectview/getdefaultresourcesheetview/)() | Uid, संसाधन नाम, प्रकार, सामग्री लेबल, प्रारंभाक्षर, समूह, अधिकतम इकाइयाँ, मानक दर, ओवरटाइम दर, प्रति उपयोग लागत, संचित समय, बेस कैलेंडर और कोड संसाधन कॉलम शामिल करता है। |
| static [GetDefaultResourceUsageView](../../aspose.tasks.visualization/projectview/getdefaultresourceusageview/)() | Uid, name, start, finish और work resource कॉलम शामिल हैं। |
| static [GetDefaultTaskSheetView](../../aspose.tasks.visualization/projectview/getdefaulttasksheetview/)() | id, indicators, name, duration, start, finish, predecessors और resource names टास्क कॉलम शामिल हैं। |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


