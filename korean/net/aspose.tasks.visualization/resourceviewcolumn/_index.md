---
title: "클래스 ResourceViewColumn"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Visualization.ResourceViewColumn 클래스. ResourceUsage 뷰와 ResourceSheet 뷰에서 사용되는 Projects 뷰 클래스"
type: docs
weight: 3350
url: /ko/net/aspose.tasks.visualization/resourceviewcolumn/
---
## ResourceViewColumn class

ResourceUsage 보기와 ResourceSheet 보기에서 사용되는 프로젝트 보기 클래스입니다.

```csharp
public sealed class ResourceViewColumn : ViewColumn
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [ResourceViewColumn](resourceviewcolumn/#constructor)(int, Field) | `ResourceViewColumn` 클래스의 새 인스턴스를 초기화합니다. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_1)(string, int, ResourceToColumnTextConverter) | `ResourceViewColumn` 클래스의 새 인스턴스를 초기화합니다. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_2)(string, int, ResourceToColumnTextConverter, Field) | `ResourceViewColumn` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/resourceviewcolumn/field/) { get; set; } | 열 필드. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | 열 이름을 가져옵니다. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | 텍스트 정렬을 가져오거나 설정합니다([`HorizontalStringAlignment`](../horizontalstringalignment/) 열거형의 값 중 하나일 수 있음). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | 열 셀의 모양을 사용자 지정하는 데 사용할 수 있는 콜백을 가져오거나 설정합니다. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | 열 너비를 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/resourceviewcolumn/getcolumntext/)(Resource) | 현재 리소스를 열 텍스트로 변환합니다. |

## 예제

내보낼 리소스 뷰 열을 추가하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);

var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new ResourceViewColumn(100, Field.ResourceName),
    new ResourceViewColumn(100, Field.ResourceActualWork),
    new ResourceViewColumn(100, Field.ResourceCost),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }, 
        Field.ResourceCost2)
};

// 열을 반복합니다
foreach (var column in columns)
{
    var col = (ResourceViewColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(resource));
    Console.WriteLine();
}

options.View = new ProjectView(columns);
options.PresentationFormat = PresentationFormat.ResourceUsage;
project.Save(OutDir + "WorkWithAssignmentViewColumn_out.pdf", options);
```

### 또 보기

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


