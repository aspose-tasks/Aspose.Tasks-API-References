---
title: "डेलीगेट AssignmentToColumnTextConverter"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceAssignment डेटा को कॉलम स्ट्रिंग में परिवर्तित करने वाला"
type: docs
weight: 2920
url: /hi/net/aspose.tasks.visualization/assignmenttocolumntextconverter/
---
## AssignmentToColumnTextConverter delegate

ResourceAssignment डेटा को कॉलम की स्ट्रिंग में बदलने वाला कन्वर्टर।

```csharp
public delegate string AssignmentToColumnTextConverter(ResourceAssignment assignment);
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| असाइनमेंट | ResourceAssignment | परिवर्तित करने के लिए असाइनमेंट। |

### रिटर्न वैल्यू

कॉलम के लिए स्ट्रिंग डेटा।

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

* class [ResourceAssignment](../../aspose.tasks/resourceassignment/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


