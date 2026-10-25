---
title: "ResourceViewColumn.GetColumnText"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceViewColumn 메서드. 현재 리소스를 열 텍스트로 변환합니다"
type: docs
weight: 30
url: /ko/net/aspose.tasks.visualization/resourceviewcolumn/getcolumntext/
---
## ResourceViewColumn.GetColumnText method

현재 리소스를 열 텍스트로 변환합니다.

```csharp
public string GetColumnText(Resource resource)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 리소스 | 리소스 | 현재 리소스. |

### 반환 값

열 텍스트.

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

* class [Resource](../../../aspose.tasks/resource/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)


