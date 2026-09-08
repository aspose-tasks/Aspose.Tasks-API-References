---
title: "AssignmentViewColumn.GetColumnText"
second_title: "Aspose.Tasks for .NET API 참조"
description: "AssignmentViewColumn 메서드. 현재 리소스 할당을 열 텍스트로 변환합니다"
type: docs
weight: 30
url: /ko/net/aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/
---
## AssignmentViewColumn.GetColumnText method

현재 리소스 할당을 열 텍스트로 변환합니다.

```csharp
public string GetColumnText(ResourceAssignment assignment)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 할당 | ResourceAssignment | 현재 할당. |

### 반환 값

열 텍스트.

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

* class [ResourceAssignment](../../../aspose.tasks/resourceassignment/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


