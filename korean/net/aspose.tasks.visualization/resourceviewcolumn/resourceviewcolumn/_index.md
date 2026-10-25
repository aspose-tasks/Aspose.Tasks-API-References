---
title: "ResourceViewColumn.ResourceViewColumn"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceViewColumn 생성자. ResourceViewColumn 클래스의 새 인스턴스를 초기화합니다"
type: docs
weight: 10
url: /ko/net/aspose.tasks.visualization/resourceviewcolumn/resourceviewcolumn/
---
## ResourceViewColumn(string, int, ResourceToColumnTextConverter, Field) {#constructor_2}

[`ResourceViewColumn`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public ResourceViewColumn(string name, int width, ResourceToColumnTextConverter converter, 
    Field field)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | 문자열 | 열 이름. |
| 너비 | Int32 | 열의 너비(픽셀). |
| 변환기 | ResourceToColumnTextConverter | 리소스 데이터를 열 텍스트로 변환하는 변환기. |
| 필드 | 필드 | 열 필드. |

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

* delegate [ResourceToColumnTextConverter](../../resourcetocolumntextconverter/)
* enum [Field](../../../aspose.tasks/field/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## ResourceViewColumn(string, int, ResourceToColumnTextConverter) {#constructor_1}

[`ResourceViewColumn`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public ResourceViewColumn(string name, int width, ResourceToColumnTextConverter converter)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | 문자열 | 열 이름. |
| 너비 | Int32 | 열의 너비(픽셀). |
| 변환기 | ResourceToColumnTextConverter | 리소스 데이터를 열 텍스트로 변환하는 변환기. |

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

* delegate [ResourceToColumnTextConverter](../../resourcetocolumntextconverter/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)

---

## ResourceViewColumn(int, Field) {#constructor}

[`ResourceViewColumn`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public ResourceViewColumn(int width, Field field)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 너비 | Int32 | 열 너비(픽셀). |
| 필드 | 필드 | 열 필드. |

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

* enum [Field](../../../aspose.tasks/field/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)


