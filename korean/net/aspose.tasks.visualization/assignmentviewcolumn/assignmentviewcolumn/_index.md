---
title: "AssignmentViewColumn.AssignmentViewColumn"
second_title: "Aspose.Tasks for .NET API 참조"
description: "AssignmentViewColumn 생성자. AssignmentViewColumn 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.visualization/assignmentviewcolumn/assignmentviewcolumn/
---
## AssignmentViewColumn constructor

AssignmentViewColumn 클래스의 새 인스턴스를 초기화합니다.

```csharp
public AssignmentViewColumn(string name, int width, AssignmentToColumnTextConverter converter)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | 문자열 | 열 이름. |
| 너비 | Int32 | 열의 너비(픽셀). |
| 변환기 | AssignmentToColumnTextConverter | 할당 데이터를 열 텍스트로 변환하는 변환기. |

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

* delegate [AssignmentToColumnTextConverter](../../assignmenttocolumntextconverter/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


