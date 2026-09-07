---
title: "AssignmentViewColumn.GetColumnText"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "AssignmentViewColumn मेथड। वर्तमान रिसोर्स असाइनमेंट को कॉलम टेक्स्ट में बदलता है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/
---
## AssignmentViewColumn.GetColumnText method

वर्तमान संसाधन असाइनमेंट को कॉलम टेक्स्ट में परिवर्तित करता है।

```csharp
public string GetColumnText(ResourceAssignment assignment)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| असाइनमेंट | ResourceAssignment | वर्तमान असाइनमेंट। |

### रिटर्न वैल्यू

कॉलम टेक्स्ट।

## उदाहरण

दिखाता है कि असाइनमेंट दृश्य के लिए कॉलम कैसे जोड़ें।

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new Spreadsheet2003SaveOptions();

var column = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(column);

foreach (var assignment in project.ResourceAssignments)
{
    foreach (var col in options.AssignmentView.Columns)
    {
        var assnCol = (AssignmentViewColumn)col;
        Console.WriteLine("Column Field: " + assnCol.Field);
        Console.WriteLine("Column Text ( converted ): " + assnCol.GetColumnText(assignment));
        Console.WriteLine();
    }
}

project.Save(OutDir + "UsingSpreadsheet2003SaveOptions_out.xml", options);
```

### संबंधित देखें

* class [ResourceAssignment](../../../aspose.tasks/resourceassignment/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


