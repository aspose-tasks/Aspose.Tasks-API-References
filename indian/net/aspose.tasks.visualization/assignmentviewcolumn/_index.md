---
title: "क्लास AssignmentViewColumn"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.AssignmentViewColumn क्लास। प्रोजेक्ट्स व्यू क्लास"
type: docs
weight: 2930
url: /hi/net/aspose.tasks.visualization/assignmentviewcolumn/
---
## AssignmentViewColumn class

प्रोजेक्ट का दृश्य वर्ग।

```csharp
public class AssignmentViewColumn : ViewColumn
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [AssignmentViewColumn](assignmentviewcolumn/)(string, int, AssignmentToColumnTextConverter) | AssignmentViewColumn क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/assignmentviewcolumn/field/) { get; set; } | कॉलम फ़ील्ड। [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | कॉलम का नाम प्राप्त करता है। |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | पाठ की संरेखण प्राप्त करता है या सेट करता है (यह [`HorizontalStringAlignment`](../horizontalstringalignment/) enumeration के मानों में से एक हो सकता है)। |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | कॉलम की कोशिकाओं की उपस्थिति को अनुकूलित करने के लिए उपयोग की जा सकने वाली कॉलबैक प्राप्त करता है या सेट करता है। |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | कॉलम की चौड़ाई प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/)(ResourceAssignment) | वर्तमान संसाधन असाइनमेंट को कॉलम टेक्स्ट में परिवर्तित करता है। |

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

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


