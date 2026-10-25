---
title: "클래스 AssignmentViewColumn"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.AssignmentViewColumn 클래스. 프로젝트 보기 클래스"
type: docs
weight: 2930
url: /ko/net/aspose.tasks.visualization/assignmentviewcolumn/
---
## AssignmentViewColumn class

프로젝트 보기 클래스.

```csharp
public class AssignmentViewColumn : ViewColumn
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [AssignmentViewColumn](assignmentviewcolumn/)(string, int, AssignmentToColumnTextConverter) | AssignmentViewColumn 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/assignmentviewcolumn/field/) { get; set; } | 열 필드. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | 열 이름을 가져옵니다. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | 텍스트 정렬을 가져오거나 설정합니다([`HorizontalStringAlignment`](../horizontalstringalignment/) 열거형의 값 중 하나일 수 있음). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | 열 셀의 모양을 사용자 지정하는 데 사용할 수 있는 콜백을 가져오거나 설정합니다. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | 열 너비를 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/)(ResourceAssignment) | 현재 리소스 할당을 열 텍스트로 변환합니다. |

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

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


