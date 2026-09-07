---
title: "SaveOptions.View"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "SaveOptions प्रॉपर्टी। यह रेंडर करने के लिए view कॉलम की सूची (GanttChartColumn) प्राप्त करता है या सेट करता है। यदि सेट नहीं किया गया है तो केवल टास्क आईडी, टास्क नाम, प्रारंभ और समाप्ति रेंडर होते हैं। यदि View और ViewSettings दोनों प्रॉपर्टी सेट हैं तो View के कॉलम ViewSettings के कॉलम को ओवरराइड करते हैं।"
type: docs
weight: 230
url: /hi/net/aspose.tasks.saving/saveoptions/view/
---
## SaveOptions.View property

रेंडर करने के लिए view कॉलम की सूची प्राप्त करता है या सेट करता है ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/))। यदि सेट नहीं किया गया है तो केवल टास्क आईडी, टास्क नाम, प्रारंभ और समाप्ति रेंडर होते हैं। यदि View और [`ViewSettings`](../viewsettings/) दोनों प्रॉपर्टी सेट हैं, तो View के कॉलम ViewSettings के कॉलम को ओवरराइड करते हैं।

```csharp
public ProjectView View { get; set; }
```

## उदाहरण

दिखाता है कि प्रोजेक्ट निर्यात के दौरान निर्यात किए जाने वाले view के कॉलम कैसे जोड़े जाएँ।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new Spreadsheet2003SaveOptions();
var ganttChartColumn = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(ganttChartColumn);

var resourceViewColumn = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(resourceViewColumn);

var assignmentViewColumn = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assignmentViewColumn);

project.Save(OutDir + "UsingSpreadsheet2003SaveOptions_out.xml", options);
```

### संबंधित देखें

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


