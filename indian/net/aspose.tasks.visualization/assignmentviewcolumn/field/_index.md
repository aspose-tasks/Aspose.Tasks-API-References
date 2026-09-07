---
title: "AssignmentViewColumn.Field"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "AssignmentViewColumn प्रॉपर्टी। कॉलम फ़ील्ड। फ़ील्ड"
type: docs
weight: 20
url: /hi/net/aspose.tasks.visualization/assignmentviewcolumn/field/
---
## AssignmentViewColumn.Field property

कॉलम फ़ील्ड। `Field`।

```csharp
public override Field Field { get; set; }
```

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

* enum [Field](../../../aspose.tasks/field/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


