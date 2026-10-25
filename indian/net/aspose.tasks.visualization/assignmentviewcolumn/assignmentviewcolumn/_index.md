---
title: "AssignmentViewColumn.AssignmentViewColumn"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "AssignmentViewColumn कंस्ट्रक्टर। AssignmentViewColumn क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.visualization/assignmentviewcolumn/assignmentviewcolumn/
---
## AssignmentViewColumn constructor

AssignmentViewColumn क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है।

```csharp
public AssignmentViewColumn(string name, int width, AssignmentToColumnTextConverter converter)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | स्ट्रिंग | कॉलम का नाम। |
| चौड़ाई | Int32 | कॉलम की चौड़ाई पिक्सेल में। |
| कनवर्टर | AssignmentToColumnTextConverter | असाइनमेंट डेटा को कॉलम टेक्स्ट में बदलने वाला कनवर्टर। |

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

* delegate [AssignmentToColumnTextConverter](../../assignmenttocolumntextconverter/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


