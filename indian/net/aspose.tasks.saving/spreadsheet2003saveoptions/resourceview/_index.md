---
title: "Spreadsheet2003SaveOptions.ResourceView"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Spreadsheet2003SaveOptions प्रॉपर्टी। रेंडर करने के लिए रिसोर्स व्यू कॉलम की सूची प्राप्त करता है या सेट करता है ResourceViewColumn"
type: docs
weight: 30
url: /hi/net/aspose.tasks.saving/spreadsheet2003saveoptions/resourceview/
---
## Spreadsheet2003SaveOptions.ResourceView property

रेंडर करने के लिए रिसोर्स व्यू कॉलम की सूची प्राप्त करता है या सेट करता है ([`ResourceViewColumn`](../../../aspose.tasks.visualization/resourceviewcolumn/)).

```csharp
public ProjectView ResourceView { get; set; }
```

## उदाहरण

दिखाता है कि कैसे प्रोजेक्ट को Spreadsheet2003 फ़ॉर्मेट में एक्सपोर्ट करते समय एक्सपोर्ट किए जाने वाले कॉलम जोड़े जाएँ।

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
* class [Spreadsheet2003SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../spreadsheet2003saveoptions/)
* assembly [Aspose.Tasks](../../../)


