---
title: "TableField 클래스"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TableField 클래스. 프로젝트의 테이블 필드를 나타냅니다."
type: docs
weight: 2340
url: /ko/net/aspose.tasks/tablefield/
---
## TableField class

프로젝트의 테이블 필드를 나타냅니다.

```csharp
public class TableField
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [TableField](tablefield/)() | `TableField` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [AlignData](../../aspose.tasks/tablefield/aligndata/) { get; set; } | 테이블 필드의 데이터 정렬을 가져오거나 설정합니다. |
| [AlignTitle](../../aspose.tasks/tablefield/aligntitle/) { get; set; } | 테이블 필드의 제목 정렬을 가져오거나 설정합니다. |
| [Field](../../aspose.tasks/tablefield/field/) { get; set; } | 테이블 필드의 유형을 가져오거나 설정합니다. |
| [Title](../../aspose.tasks/tablefield/title/) { get; set; } | 테이블 내 필드의 제목을 가져오거나 설정합니다. |
| [Width](../../aspose.tasks/tablefield/width/) { get; set; } | 테이블의 필드 열 너비(포인트)를 가져오거나 설정합니다. |
| [WrapHeader](../../aspose.tasks/tablefield/wrapheader/) { get; set; } | 테이블 열 머리글을 여러 줄로 자동 줄바꿈할지, 열 너비를 초과하면 잘라낼지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [WrapText](../../aspose.tasks/tablefield/wraptext/) { get; set; } | 열 텍스트가 여러 줄로 자동 줄바꿈될 수 있는지, 또는 열 너비를 초과할 경우 잘려야 하는지를 나타내는 값을 가져오거나 설정합니다. MSP 2010 버전 및 이후 버전에서 지원됩니다. |

## 예제

Project의 뷰를 작업하고 기본 뷰에 열을 추가하는 방법을 보여줍니다(이는 MPP 파일을 MS Project에서 열었을 때 표시되는 뷰입니다).

```csharp
// 뷰 없이 빈 프로젝트를 생성합니다.
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// 기본 뷰를 수정합니다(이 뷰는 간트 차트 뷰입니다).
// 또는 project.View 컬렉션을 사용하여 이름이나 View Screen으로 뷰를 선택할 수 있습니다.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// WriteViewData 플래그는 뷰 속성의 수정 사항을 영구히 저장하는 데 사용해야 합니다.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

프로젝트 테이블을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// 테이블을 가져옵니다.
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// 모든 테이블 필드 정보를 표시합니다.
foreach (var field in table.TableFields)
{
    Console.WriteLine("  Field: " + field.Field);
    Console.WriteLine("  Width: " + field.Width);
    Console.WriteLine("  Title: " + field.Title);
    Console.WriteLine("  Title Alignment: " + field.AlignTitle);
    Console.WriteLine("  Data Alignment: " + field.AlignData);
    Console.WriteLine("  Wrap Header: " + field.WrapHeader);
    Console.WriteLine("  Wrap Text: " + field.WrapText);
    Console.WriteLine();
}
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


