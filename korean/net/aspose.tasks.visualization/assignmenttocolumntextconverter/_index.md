---
title: "델리게이트 AssignmentToColumnTextConverter"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceAssignment 데이터를 열 문자열 변환기로 변환"
type: docs
weight: 2920
url: /ko/net/aspose.tasks.visualization/assignmenttocolumntextconverter/
---
## AssignmentToColumnTextConverter delegate

ResourceAssignment 데이터를 열 문자열로 변환합니다.

```csharp
public delegate string AssignmentToColumnTextConverter(ResourceAssignment assignment);
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 할당 | ResourceAssignment | 변환할 할당입니다. |

### 반환 값

열에 대한 문자열 데이터.

## 예제

할당 보기용 열을 추가하는 방법을 보여줍니다.

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

### 또 보기

* class [ResourceAssignment](../../aspose.tasks/resourceassignment/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


